<script>
    export let y;
    export let innerHeight;

    export let tabs = [
        { name: "Projects", link: "#projects" },
        { name: "About me", link: "#about" },
        { name: "Blog", link: "https://medium.com/@dikshanthere2", target: "_blank" },
        { name: "Resume", link: "/images/dikshant-resume.pdf", target: "_blank" }
    ];
</script>

<header
    class={"sticky z-[10] top-0 duration-200 px-6 flex items-center justify-between border-b border-solid " +
        (y > 0
            ? " py-4 bg-slate-950 border-violet-950"
            : " py-6 bg-transparent border-transparent")}
>
    <h1 class="font-medium">
        <b class="font-bold poppins">Dikshant</b> <span>Choudhary</span>
    </h1>

    <div class="sm:flex items-center gap-4 hidden">
        {#each tabs as tab}
            <a
                href={tab.link}
                class="duration-200 hover:text-violet-400"
                target={tab.target || ""}
                rel={tab.target === "_blank" ? "noopener noreferrer" : ""}
            >
                <p>{tab.name}</p>
            </a>
        {/each}
        <a href="https://wa.me/919461921220" target="_blank">
    <button
        class="blueShadow relative overflow-hidden px-5 py-2 group rounded-full bg-white text-slate-950 flex items-center gap-2"
    >
        <div
            class="absolute top-0 right-full w-full h-full bg-violet-400 opacity-20 group-hover:translate-x-full z-0 duration-200"
        ></div>
        <h4 class="relative z-10">Hire Me</h4>
        <i class="fa-solid fa-fire relative z-10 text-red-500"></i>
    </button>
</a>
</header>
