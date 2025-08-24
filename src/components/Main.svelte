<script>
    import Step from "./Step.svelte";

    let steps = [
        {
            name: "Dikshant Store",
            icon: "fa-solid fa-cart-shopping",
            description:
                "Smoljames Store is a a merchanising store created with Next.js, Commerce.js & Stripe! Commerce.js is a CMS for managing project and Stripe is used for all transaction handling.",
        },
        {
            name: "Utlimate Todos",
            icon: "fa-solid fa-list-check",
            description:
                "Test for model robustness with customized test profiles and receive exhaustive reporting on the performance and potential vulnerabilities of your model.",
        },
        {
            name: "Pokédex",
            icon: "fa-solid fa-diagram-project",
            description:
                "Augment your datasets with our filters and dataset manipulations to ensure your models are trained on the highest quality datasets (coming soon).",
        },
        {
            name: "Pokédex",
            icon: "fa-solid fa-diagram-project",
            description:
                "Augment your datasets with our filters and dataset manipulations to ensure your models are trained on the highest quality datasets (coming soon).",
        },
    ];

    let benefits = [
        {
            metric: "10x",
            name: "a self taught developer",
            description:
                "I taught myself to code using free online resources and absolutely fell in love with the creativity and problem solving that is involved in developing and engineering innovative new online experiences. Starting of with JavaScript, HTML & CSS and evolving my knowledge base to include JavaScript frameworks, backend programming, design, cloud services and much much more.",
        },
        {
            name: "a product design & UX finatic",
            description:
                "Carefully crafting and designing amazing user experiences allows me to express and experiment with every morsel of creativity I have. I love the challenge of learning new design concepts and enabling users with amazing online experiences.",
        },
        {
            name: "an excellent communicator",
            description:
                "Communication is key and it's a paramount value of mine. I believe in transparency and constructive communication above all else. This helps me develop deep relationships and ensures my effectiveness and productivity in any work space with any team.",
        },
    ];

    let skills = [
        {
            name: "HTML",
            icon: "fa-brands fa-html5",
            description:
                "Proficient in HTML5 for structuring and presenting content on the web.",
        },
        {
            name: "CSS",
            icon: "fa-brands fa-css3-alt",
            description:
                "Skilled in CSS3 for styling and layout of web pages, including responsive design.",
        },
        {
            name: "JavaScript",
            icon: "fa-brands fa-js",
            description:
                "Experienced in JavaScript for adding interactivity and functionality to web applications.",
        },
        {
            name: "MERN Stack",
            icon: "fa-brands fa-react",
            description:
                "Full-stack development using MongoDB, Express.js, React, and Node.js.",
        },
        {
            name: "Content Writing",
            icon: "fa-solid fa-pen-nib",
            description:
                "Creating engaging and informative content for various platforms.",
        },
        {
            name: "Copywriting",
            icon: "fa-solid fa-pencil",
            description:
                "Crafting persuasive copy for marketing and advertising purposes.",
        },
        {
            name: "Excel",
            icon: "fa-solid fa-table",
            description:
                "Advanced skills in Microsoft Excel for data analysis, formulas, and dashboards.",
        },
        {
            name: "Power BI",
            icon: "fa-solid fa-chart-pie",
            description:
                "Proficient in Power BI for data visualization and business intelligence reporting.",
        },
        {
            name: "SQL",
            icon: "fa-solid fa-database",
            description:
                "Experienced in SQL for querying and managing relational databases.",
        },
        {
            name: "Digital Marketing",
            icon: "fa-solid fa-bullhorn",
            description:
                "Knowledgeable in digital marketing strategies, SEO, social media, and analytics.",
        },
    ];

    let certifications = [
        {
            name: "Google Data Analytics Certificate",
            icon: "fa-solid fa-chart-bar",
            description:
                "Completed the Google Data Analytics Professional Certificate, covering data cleaning, analysis, and visualization using tools like SQL, Excel, and Tableau.",
        },
        {
            name: "Microsoft Certified: Azure Fundamentals",
            icon: "fa-solid fa-cloud",
            description:
                "Earned certification in Azure cloud services, understanding core concepts of cloud computing.",
        },
        {
            name: "HubSpot Content Marketing Certification",
            icon: "fa-solid fa-pen",
            description:
                "Certified in content marketing strategies, SEO, and creating valuable content.",
        },
        {
            name: "freeCodeCamp Full Stack Development",
            icon: "fa-solid fa-code",
            description:
                "Completed certifications in Responsive Web Design, JavaScript Algorithms, Front End Libraries, Data Visualization, APIs and Microservices, and more.",
        },
    ];

    let testimonials = [
        {
            name: "John Doe",
            icon: "fa-solid fa-quote-left",
            description:
                "Dikshant is an excellent developer who delivered our project on time with great quality. His problem-solving skills are impressive!",
            image: "https://pravatar.cc/150?img=1"
        },
        {
            name: "Jane Smith",
            icon: "fa-solid fa-quote-left",
            description:
                "Working with Dikshant was a pleasure; his communication skills are top-notch and he always goes the extra mile.",
            image: "https://pravatar.cc/150?img=2"
        },
        {
            name: "Alex Johnson",
            icon: "fa-solid fa-quote-left",
            description:
                "The insights from the data analysis Dikshant provided transformed our business decisions. Highly recommended!",
            image: "https://pravatar.cc/150?img=3"
        },
        {
            name: "Emily Davis",
            icon: "fa-solid fa-quote-left",
            description:
                "Dikshant's copywriting and digital marketing expertise helped boost our online presence significantly.",
            image: "https://pravatar.cc/150?img=4"
        },
    ];
</script>

<main class="flex flex-col flex-1 p-4">
    <section
        id="introPage"
        class="grid grid-cols-1 lg:grid-cols-2 gap-10 py-8 sm:py-14"
    >
        <div
            class="flex flex-col lg:justify-center text-center lg:text-left gap-6 md:gap-8 lg:gap-10"
        >
            <h2 class="font-semibold text-4xl sm:text-5xl md:text-6xl">
                Hi! I'm <span class="poppins text-violet-400">Dikshant</span> Choudhary
                <!-- <br />Full Stack
                <span class="poppins text-violet-400">Developer</span> -->
            </h2>
            <p class="text-base sm:text-lg md:text-xl">
                  I’m a <span class="text-violet-400">self-taught software developer</span> passionate about 
                  problem-solving, design, and technology. Experienced in full-stack 
                  development with JavaScript, Node.js, and modern web technologies.
              </p>

              <p class="text-base sm:text-lg md:text-xl">
                  Also a Data Analyst skilled in <span class="text-violet-400">Excel dashboards, SQL, and Power BI</span>, 
                  turning data into actionable insights. Additionally experienced in 
                  <span class="text-violet-400">copywriting, content writing, and digital marketing</span> 
                  with a strong record of leadership and project success.
              </p>
            <a
                href="/contact"
                class="blueShadow mx-auto lg:mr-auto lg:ml-0 text-base sm:text-lg md:text-xl poppins relative overflow-hidden px-6 py-3 group rounded-full bg-white text-slate-950"
            >
                <div
                    class="absolute top-0 right-full w-full h-full bg-violet-400 opacity-20 group-hover:translate-x-full z-0 duration-200"
                />
                <h4 class="relative z-9">Get in touch &rarr;</h4>
            </a>
        </div>
        
        <div class="relative shadow-2xl grid place-items-center">
            <img
                src={"images/p.jpeg"}
                alt="Zetane Engine"
                class="object-cover z-[2] max-h-[70vh]"
            />
        </div>
        <!-- <div  class="flex p-0.5 relative max-w-[700px] w-full mx-auto">
            <div
                class="absolute inset-0 overflow-hidden rounded-md flex items-center justify-center"
            >
                <div
                    class="bg-gradient-to-r absolute inset-[-20px]  from-violet-800 to-indigo-800 specialSpin"
                />
            </div>

            <img
                src={"images/zetane-engine.jpeg"}
                alt="Zetane Engine"
                class="w-full h-full object-cover z-[2]"
            />
        </div> -->
    </section>
    <section class="py-20 lg:py-32 flex flex-col gap-24" id="projects">
        <div class="flex flex-col gap-2 text-center">
            <h6 class="text-large sm:text-xl md:text-2xl">
                A few of my creative endeavors.
            </h6>
            <h3 class="font-semibold text-3xl sm:text-4xl md:text-5xl">
                Curious to <span class="poppins text-violet-400">see</span> my work?
            </h3>
        </div>
        <a
            href="https://www.youtube.com/watch?v=dQw4w9WgXcQ"
            target="_blank"
            class="mx-auto px-4 py-2 rounded-md border border-solid border-white flex items-center gap-2 -mb-4 sm:-mb-0 -mt-10 hover:border-violet-700 duration-200"
        >
            <i class="fa-regular fa-circle-play" />
            <p>Watch the video</p>
        </a>
        <div class="grid grid-cols-1 lg:grid-cols-4 gap-12 lg:gap-10">
            <Step step={steps[0]}>
                <p>
                    Smoljames Store is a a merchanising store created with <strong
                        class="text-violet-400"
                        >Next.js, Commerce.js, Stripe & Node.js + Express.js!</strong
                    > Commerce.js is a product CMS and Stripe is used for all transaction
                    handling.
                </p>
            </Step>
            <Step step={steps[1]}>
                <p>
                    Ultimate Todos is a Full Stack <strong
                        class="text-violet-400">Next.js</strong
                    >,
                    <strong class="text-violet-400">Node.js + Express.js</strong
                    >
                    & <strong class="text-violet-400">Firebase</strong> CRUD application
                    that allows a user to login, manage a tidy and efficacious todo
                    list, and persist this information across devices.
                </p>
            </Step>
            <Step step={steps[2]}>
                <p>
                    The Pokédex is a <strong class="text-violet-400"
                        >SvelteKit & TailwindCSS</strong
                    >
                    web application, hosted on
                    <strong class="text-violet-400">Netlify</strong>, that
                    consumes and caches the
                    <strong class="text-violet-400">Pokémon API</strong>
                    to display all Pokémon information. Gotta catch them all!
                </p>
            </Step>
            <Step step={steps[3]}>
                <p>
                    The Pokédex is a <strong class="text-violet-400"
                        >SvelteKit & TailwindCSS</strong
                    >
                    web application, hosted on
                    <strong class="text-violet-400">Netlify</strong>, that
                    consumes and caches the
                    <strong class="text-violet-400">Pokémon API</strong>
                    to display all Pokémon information. Gotta catch them all!
                </p>
            </Step>
        </div>
    </section>
    <section
        id="about"
        class="py-20 pt-10 lg:pt-16 lg:py-32 flex flex-col gap-16 sm:gap-20 md:gap-24 relative"
    >
        <!-- <div class="z-[-1] bg-violet-950 w-screen left-1/2 -translate-x-1/2 top-0 h-full absolute"> </div> -->
        <div
            class="flex flex-col gap-2 text-center relative before:absolute before:top-0 before:left-0 before:w-2/3 before:h-1.5 before:bg-violet-700 after:absolute after:bottom-0 after:right-0 after:w-2/3 after:h-1.5 after:bg-violet-700 py-4"
        >
            <h6 class="text-large sm:text-xl md:text-2xl">
                Want to know more?
            </h6>
            <h3 class="font-semibold text-3xl sm:text-4xl md:text-5xl">
                A bit <span class="poppins text-violet-400">about</span> me.
            </h3>
        </div>
        <p class="mx-auto poppins font-semibold text-lg sm:text-xl md:text-2xl">
            I am . . .
        </p>
        <div class="flex flex-col gap-20 w-full mx-auto max-w-[800px]">
            {#each benefits as benefit, index}
                <!-- <div class="flex flex-col gap-2 mx-auto">
                    <div class="flex items-end gap-4">
                        <p
                            class="poppins text-6xl sm:text-7xl md:text-8xl text-slate-500 font-medium"
                        >
                            {benefit.metric}
                        </p>
                        <p
                            class="text-xl sm:text-2xl md:text-3xl capitalize pb-2"
                        >
                            {benefit.name}
                        </p>
                    </div>
                    <p class="text-center italic">- {benefit.description}</p>
                </div> -->
                <div class="flex gap-6 sm:gap-8">
                    <p
                        class="poppins text-4xl sm:text-5xl md:text-6xl text-slate-500 font-semibold"
                    >
                        0{index + 1}
                    </p>
                    <div class="flex flex-col gap-6 sm:gap-8">
                        <h3 class="text-2xl sm:text-3xl md:text-5xl">
                            {benefit.name}
                        </h3>
                        <p>{benefit.description}</p>
                    </div>
                </div>
            {/each}
        </div>
        <h5 class={" text-2xl sm:text-3xl font-semibold text-center poppins "}>
            The <span class="text-violet-400">Complete</span> Package
        </h5>
        <div
            class="flex flex-col overflow-x-scroll gap-10 max-w-[800px] mx-auto w-full"
        >
            <table class="bg-white text-slate-700 rounded text-center">
                <thead class={"border-b border-solid border-slate-200  "}>
                    <tr class="">
                        <th />
                        <th class="whitespace-nowrap p-2 px-4">Candidate #1</th>
                        <th class="whitespace-nowrap p-2 px-4">Candidate #2</th>
                        <th class="whitespace-nowrap p-2 px-4">Candidate #3</th>
                        <th
                            class="bg-violet-700 text-white whitespace-nowrap p-4 px-8"
                            >Me</th
                        >
                    </tr>
                </thead>
                <tbody>
                    <tr class="border-b border-solid border-slate-200">
                        <td
                            class="border-r border-solid border-white pl-4 pr-8 py-4 font-semibold text-sm"
                            >Dedication</td
                        >
                        <td><i class="fa-solid fa-xmark text-slate-500" /></td>
                        <td><i class="fa-solid fa-check text-slate-500" /></td>
                        <td><i class="fa-solid fa-xmark text-slate-500" /></td>
                        <td><i class="fa-solid fa-check text-green-500" /></td>
                    </tr>
                    <tr class="border-b border-solid border-slate-200">
                        <td
                            class="border-r border-solid border-white pl-4 pr-8 py-4 font-semibold text-sm"
                            >Critical Thought</td
                        >
                        <td><i class="fa-solid fa-xmark text-slate-500" /></td>
                        <td><i class="fa-solid fa-check text-slate-500" /></td>
                        <td><i class="fa-solid fa-check text-slate-500" /></td>
                        <td><i class="fa-solid fa-check text-green-500" /></td>
                    </tr>
                    <tr>
                        <td
                            class="border-r border-solid border-white pl-4 pr-8 py-4 font-semibold text-sm"
                            >Interpersonal Skills</td
                        >
                        <td><i class="fa-solid fa-check text-slate-500" /></td>
                        <td><i class="fa-solid fa-check text-slate-500" /></td>
                        <td><i class="fa-solid fa-xmark text-slate-500" /></td>
                        <td><i class="fa-solid fa-check text-green-500" /></td>
                    </tr>
                    <tr class="border-t border-solid border-slate-200">
                        <td
                            class="border-r border-solid border-white pl-4 pr-8 py-4 font-semibold text-sm"
                            >Progamming Ability</td
                        >
                        <td><i class="fa-solid fa-check text-slate-500" /></td>
                        <td><i class="fa-solid fa-xmark text-slate-500" /></td>
                        <td><i class="fa-solid fa-check text-slate-500" /></td>
                        <td><i class="fa-solid fa-check text-green-500" /></td>
                    </tr>
                </tbody>
            </table>
        </div>
        <div class="mx-auto -mt-12 italic sm:hidden opacity-50">
            <p>Scroll to see more &rarr;</p>
        </div>
        <p class="mx-auto">So why not invest?</p>
    </section>
    <section id="skills" class="py-20 lg:py-32 flex flex-col gap-24">
        <div class="flex flex-col gap-2 text-center">
            <h6 class="text-large sm:text-xl md:text-2xl">
                My technical and professional expertise.
            </h6>
            <h3 class="font-semibold text-3xl sm:text-4xl md:text-5xl">
                My <span class="poppins text-violet-400">Skills</span>
            </h3>
        </div>
        <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 xl:grid-cols-5 gap-12 lg:gap-10">
            {#each skills as skill}
                <Step step={skill} />
            {/each}
        </div>
    </section>
    <section id="certifications" class="py-20 lg:py-32 flex flex-col gap-24">
        <div class="flex flex-col gap-2 text-center">
            <h6 class="text-large sm:text-xl md:text-2xl">
                Certified by the best.
            </h6>
            <h3 class="font-semibold text-3xl sm:text-4xl md:text-5xl">
                My <span class="poppins text-violet-400">Certifications</span>
            </h3>
        </div>
        <div class="grid grid-cols-1 lg:grid-cols-4 gap-12 lg:gap-10">
            {#each certifications as cert}
                <Step step={cert} />
            {/each}
        </div>
    </section>
    <section id="testimonials" class="py-20 lg:py-32 flex flex-col gap-24">
        <div class="flex flex-col gap-2 text-center">
            <h6 class="text-large sm:text-xl md:text-2xl">
                What others say about me.
            </h6>
            <h3 class="font-semibold text-3xl sm:text-4xl md:text-5xl">
                <span class="poppins text-violet-400">Testimonials</span>
            </h3>
        </div>
        <div class="grid grid-cols-1 lg:grid-cols-4 gap-12 lg:gap-10">
            {#each testimonials as test}
                <Step step={test}>
                    <img src={test.image} alt={test.name} class="w-16 h-16 rounded-full mx-auto mb-4" />
                    <p class="italic">"{test.description}"</p>
                </Step>
            {/each}
        </div>
    </section>
</main>