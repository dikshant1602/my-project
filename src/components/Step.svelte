<script>
    export let step;
    let showModal = false;

    function toggleModal() {
        showModal = !showModal;
    }

    // This allows closing the modal by pressing the Escape key.
    function handleKeydown(event) {
        if (event.key === 'Escape') {
            showModal = false;
        }
    }
</script>

<svelte:window on:keydown={handleKeydown}/>

<div
    class="p-4 sm:p-6 flex flex-col gap-4 rounded-lg border border-solid border-violet-900 text-center group duration-200 hover:border-violet-700 hover:-translate-y-2 bg-slate-950/30"
>
    <div
        class="bg-slate-900 grid place-items-center px-4 text-5xl mx-auto duration-200 -mt-10 sm:-mt-12"
    >
        <slot name="image"></slot>
        {#if !$$slots.image}
            <i class="{step.icon} group-hover:text-violet-400 duration-200"></i>
        {/if}
    </div>
    
    <h3 class="font-medium text-xl sm:text-2xl">
        {step.name}
    </h3>

    <p class="flex-1 text-slate-300 text-sm">{step.description}</p>
    
    <div class="mt-4">
        {#if step.githubUrl}
            <a 
                href={step.githubUrl} 
                target="_blank" 
                rel="noopener noreferrer"
                class="text-violet-400 hover:text-violet-300 duration-200 font-semibold"
            >
                View on GitHub &rarr;
            </a>
        {:else if step.linkedinUrl}
            <a 
                href={step.linkedinUrl} 
                target="_blank" 
                rel="noopener noreferrer"
                class="text-violet-400 hover:text-violet-300 duration-200 font-semibold"
            >
                View on LinkedIn &rarr;
            </a>
        {:else if step.certificateImage || step.details}
            <button
                on:click={toggleModal}
                class="text-violet-400 hover:text-violet-300 duration-200 font-semibold"
            >
                View Details &rarr;
            </button>
        {/if}
    </div>
</div>

{#if showModal}
    <div
        class="fixed inset-0 bg-black bg-opacity-80 z-50 flex justify-center items-center p-4 cursor-pointer"
        on:click={toggleModal}
        role="dialog"
        aria-modal="true"
    >
        <div
            class="bg-slate-900 border border-solid border-violet-700 rounded-lg p-6 max-w-lg w-full text-center relative cursor-auto shadow-2xl shadow-violet-900/50"
            on:click|stopPropagation
        >
            <button
                on:click={toggleModal}
                class="absolute top-2 right-4 text-3xl hover:text-violet-400 duration-200 z-10"
                aria-label="Close modal"
            >
                &times;
            </button>
            <h2 class="text-3xl font-bold mb-6 text-violet-400">{step.name}</h2>
            
            {#if step.certificateImage}
                <div class="flex flex-col gap-6 items-center">
                    <img src={step.certificateImage} alt="Certificate for {step.name}" class="rounded-md border-2 border-slate-700 w-full" />
                    {#if step.credentialUrl}
                        <a href={step.credentialUrl} target="_blank" rel="noopener noreferrer" class="bg-violet-600 text-white px-6 py-2 rounded-md hover:bg-violet-500 duration-200">
                            Verify Credential
                        </a>
                    {/if}
                </div>

            {:else if step.details}
                <ul class="text-left space-y-3">
                    {#each step.details as detail}
                        <li class="text-lg bg-slate-800 p-3 rounded-md">
                            <i class="fa-solid fa-check text-green-500 mr-3"></i>{detail}
                        </li>
                    {/each}
                </ul>
            {/if}
        </div>
    </div>
{/if}