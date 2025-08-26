<script>
    import Step from "./Step.svelte";

    // --- PROJECTS ---
    // Added a `githubUrl` to each project object
    let steps = [
        {
            name: "Weapon Inventory Management",
            icon: "fa-solid fa-person-rifle",
            description:
                "Developed a secure weapon inventory system for efficient distribution and record maintenance, incorporating daily tracking and officer signatures for issuance.",
            githubUrl: "https://github.com/dikshant1602/your-repo-name",
        },
        {
            name: "Level-Up | Learning Management System",
            icon: "fa-solid fa-graduation-cap",
            description:
                "Built a web platform for course browsing, purchases, video lectures, quizzes, and progress tracking. Integrated React, Node.js, and MongoDB for a scalable and secure learning experience.",
            githubUrl: "https://github.com/dikshant1602/your-repo-name",
        },
        {
            name: "Basic Chat Application",
            icon: "fa-solid fa-comments",
            description:
                "Developed a real-time chat application with secure login and session management. Messages are stored efficiently using MySQL and work seamlessly across all major browsers.",
            githubUrl: "https://github.com/dikshant1602/your-repo-name",
        },
        {
            name: "Amazon Clone",
            icon: "fa-brands fa-amazon",
            description:
                "A fully functional e-commerce clone built with HTML, CSS, and JavaScript. Features include product listings, add-to-cart, search, and a responsive UI.",
            githubUrl: "https://github.com/dikshant1602/your-repo-name",
        },
        {
            name: "Gym Landing Page",
            icon: "fas fa-dumbbell",
            description:
                "A modern and responsive gym landing page built with Svelte, designed to showcase fitness services with a sleek UI and smooth performance. Focused on speed, interactivity, and a clean user experience.",
            githubUrl: "https://github.com/dikshant1602/your-repo-name", 
        },
        {
            name: "Power BI and Excel Dashboards",
            icon: "fa-solid fa-file-excel",
            description:
                "Developed multiple dashboards to transform raw data into actionable insights using Excel (Pivot Tables, Power Query) and Power BI (DAX, data modeling).",
            githubUrl: "https://github.com/dikshant1602/your-repo-name",
        },
    ];

    let benefits = [
        {
            metric: "10x",
            name: "A self-taught developer",
            description:
                "I taught myself to code using free online resources and absolutely fell in love with the creativity and problem-solving that is involved in developing and engineering innovative new online experiences. Starting off with JavaScript, HTML & CSS and evolving my knowledge base to include JavaScript frameworks, backend programming, design, cloud services and much much more.",
        },
        {
            name: "A product design & UX fanatic",
            description:
                "Carefully crafting and designing amazing user experiences allows me to express and experiment with every morsel of creativity I have. I love the challenge of learning new design concepts and enabling users with amazing online experiences.",
        },
        {
            name: "An excellent communicator",
            description:
                "Communication is key and it's a paramount value of mine. I believe in transparency and constructive communication above all else. This helps me develop deep relationships and ensures my effectiveness and productivity in any workspace with any team.",
        },
        {
            name: "A persuasive writer",
            description:
                "Skilled in crafting compelling narratives and persuasive content that engages audiences, drives action, and enhances marketing efforts. My writing focuses on clarity, impact, and audience resonance to achieve business goals.",
        },
        {
            name: "An expert data visualizer",
            description:
                "Skilled in transforming raw data into meaningful insights using Power BI, Excel, and SQL. I specialize in creating interactive dashboards, reports, and visualizations that simplify complex datasets, highlight key trends, and support data-driven decision making.",
        },
    ];

    // --- SKILLS ---
    let skills = [
        {
            name: "Frontend Development",
            icon: "fa-solid fa-code",
            description: "Building beautiful and responsive user interfaces.",
            details: ["HTML", "CSS", "JavaScript", "Svelte"],
        },
        {
            name: "Backend Development",
            icon: "fa-solid fa-server",
            description: "Developing robust and scalable server-side applications.",
            details: ["MERN Stack (MongoDB, Express, React, Node.js)", "Python", "SQL"],
        },
        {
            name: "Data Analysis",
            icon: "fa-solid fa-chart-line",
            description: "Transforming raw data into actionable business insights.",
            details: ["Microsoft Excel", "Power BI", "SQL"],
        },
        {
            name: "Design",
            icon: "fa-solid fa-palette",
            description: "Creating intuitive and engaging user experiences.",
            details: ["Figma (UI/UX Design)", "Framer (Prototyping)"],
        },
        {
            name: "Marketing & Content",
            icon: "fa-solid fa-bullhorn",
            description: "Crafting compelling content and driving online growth.",
            details: ["Content Writing", "Copywriting", "Digital Marketing & SEO"],
        },
    ];

    // --- CERTIFICATIONS ---
    let certifications = [
        {
            name: "Google Data Analytics Professional Certificate",
            icon: "fa-solid fa-chart-bar",
            description:
                "Completed the Google Data Analytics Professional Certificate, covering data cleaning, analysis, and visualization using tools like SQL, Excel, and Tableau.",
            certificateImage: "/images/certs/google-data-analytics.png",
            credentialUrl: "https://www.coursera.org/account/accomplishments/professional-cert/your-id",
        },
        {
            name: "Microsoft Azure Fundamentals",
            icon: "fa-solid fa-cloud",
            description:
                "Earned certification in Azure cloud services, understanding core concepts of cloud computing.",
            certificateImage: "/images/certs/azure-fundamentals.png",
            credentialUrl: "https://learn.microsoft.com/en-us/users/your-id/credentials/your-cert-id",
        },
        {
            name: "Content Marketing Certification",
            icon: "fa-solid fa-pen",
            description:
                "Certified in content marketing strategies, SEO, and creating valuable content.",
            certificateImage: "/images/certs/content-marketing.png",
            credentialUrl: "https://www.hubspot.com/your-cert-link",
        },
        {
            name: "freeCodeCamp Developer Certifications",
            icon: "fa-solid fa-code",
            description:
                "Completed certifications in Responsive Web Design, JavaScript Algorithms, Front End Libraries, Data Visualization, APIs and Microservices, and more.",
            certificateImage: "/images/certs/freecodecamp.png",
            credentialUrl: "https://www.freecodecamp.org/your-username",
        },
    ];

    // --- TESTIMONIALS ---
    let testimonials = [
        {
            name: "Dr. Mamta Rathore",
            icon: "fa-solid fa-quote-left",
            description:
                "I had the pleasure of working with Dikshant Chaudhary during his time at MLSU. Throughout our interactions, I was consistently impressed by his dedication, curiosity, and eagerness to learn.",
            image: "https://media.licdn.com/dms/image/v2/D4E03AQHsR0zqRryXmw/profile-displayphoto-shrink_100_100/B4EZTKqW_rG0AU-/0/1738566892563?e=1759363200&v=beta&t=X21ac6BRIdNQn9xRusd1DEvKma_Zg65_dznXNcqvulY",
            linkedinUrl: "https://www.linkedin.com/in/johndoe",
        },
        {
            name: "Charchit Mangal",
            icon: "fa-solid fa-quote-left",
            description:
                "Working with Dikshant was a pleasure; his communication skills are top-notch and he always goes the extra mile.",
            image: "https://media.licdn.com/dms/image/v2/D5603AQG6r_oQpqt_7g/profile-displayphoto-shrink_100_100/profile-displayphoto-shrink_100_100/0/1726934700311?e=1759363200&v=beta&t=4vtf0LDVVXTGH03qISW0o75hmwblFJEnNZErG0_VQls",
            linkedinUrl: "https://www.linkedin.com/in/janesmith",
        },
        {
            name: "Vansh Rawat",
            icon: "fa-solid fa-quote-left",
            description:
                "Worked with Dikshant on a data project and was consistently impressed by his technical skills and teamwork. He’s quick to grasp complex problems, writes clean code, and always brings valuable ideas to the table. A solid developer and a great person to work with!",
            image: "https://media.licdn.com/dms/image/v2/D4E03AQFmDP-T171d5Q/profile-displayphoto-shrink_100_100/profile-displayphoto-shrink_100_100/0/1715840035800?e=1759363200&v=beta&t=MMQgrd8qSeUNIV0QTnLj_aYc1Jb01CxiXYqeUMgUcHA",
            linkedinUrl: "https://www.linkedin.com/in/alexjohnson",
        },
        {
            name: "Snehil Sinha",
            icon: "fa-solid fa-quote-left",
            description:
                "I had the pleasure of working with Dikshant on a web development project, and he is an outstanding teammate. His technical skills, problem-solving mindset, and ability to collaborate made a big impact on our project’s success. highly recommended!",
            image: "https://media.licdn.com/dms/image/v2/C4D03AQFwIwiasWLvoA/profile-displayphoto-shrink_100_100/profile-displayphoto-shrink_100_100/0/1659416668742?e=1759363200&v=beta&t=x8-oSq3qkE-oHZCbpu6gDpsCwADB0mY4VKehVV_IP14",
            linkedinUrl: "https://www.linkedin.com/in/emilydavis",
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
                href="#contact"
                class="blueShadow mx-auto lg:mr-auto lg:ml-0 text-base sm:text-lg md:text-xl poppins relative overflow-hidden px-6 py-3 group rounded-full bg-white text-slate-950 w-fit"
            >
                <div
                    class="absolute top-0 right-full w-full h-full bg-violet-400 opacity-20 group-hover:translate-x-full z-0 duration-200"
                />
                <h4 class="relative z-10">Get in touch →</h4>
            </a>
        </div>
       
        <div class="relative shadow-2xl grid place-items-center">
            <img
                src={"/images/p.jpeg"}
                alt="Dikshant Choudhary"
                class="object-cover z-[2] max-h-[70vh] rounded-md"
            />
        </div>
    </section>

    <section class="py-20 lg:py-32 flex flex-col gap-16" id="projects">
        <div class="flex flex-col gap-2 text-center">
            <h6 class="text-large sm:text-xl md:text-2xl">
                A few of my creative endeavors.
            </h6>
            <h3 class="font-semibold text-3xl sm:text-4xl md:text-5xl">
                Curious to <span class="poppins text-violet-400">see</span> my work?
            </h3>
        </div>
        
        <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-12 lg:gap-10">
            {#each steps as step}
                <Step {step} />
            {/each}
        </div>

        <a href="https://github.com/dikshant1602" target="_blank" rel="noopener noreferrer" class="mx-auto mt-4 px-6 py-3 rounded-md border border-solid border-white flex items-center gap-3 hover:border-violet-700 hover:bg-violet-900/20 duration-200">
            <i class="fa-brands fa-github"></i>
            <p>View More Projects on GitHub</p>
        </a>
    </section>

    <section
        id="about"
        class="py-20 pt-10 lg:pt-16 lg:py-32 flex flex-col gap-16 sm:gap-20 md:gap-24 relative"
    >
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
        
        <div class="flex flex-col gap-16 w-full mx-auto max-w-[800px]">
            {#each benefits as benefit, index}
                <div class="flex gap-6 sm:gap-8 items-start">
                    <p class="poppins text-4xl sm:text-5xl md:text-6xl text-slate-600 font-semibold">
                        0{index + 1}
                    </p>
                    <div class="flex flex-col gap-4">
                        <h3 class="text-2xl sm:text-3xl md:text-4xl poppins font-semibold">
                            {benefit.name}
                        </h3>
                        <p class="text-slate-300">{benefit.description}</p>
                    </div>
                </div>
            {/each}
        </div>

        <div class="flex flex-col gap-8 items-center">
            <h5 class={" text-2xl sm:text-3xl font-semibold text-center poppins "}>
                The <span class="text-violet-400">Complete</span> Package
            </h5>
            <div
                class="flex flex-col overflow-x-auto gap-10 max-w-[800px] mx-auto w-full"
            >
                <table class="bg-white text-slate-700 rounded text-center w-full">
                    <thead class={"border-b border-solid border-slate-200"}>
                        <tr>
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
                                class="border-r border-solid border-white pl-4 pr-8 py-4 font-semibold text-sm text-left"
                                >Dedication</td
                            >
                            <td><i class="fa-solid fa-xmark text-slate-500" /></td>
                            <td><i class="fa-solid fa-check text-slate-500" /></td>
                            <td><i class="fa-solid fa-xmark text-slate-500" /></td>
                            <td><i class="fa-solid fa-check text-green-500 text-lg" /></td>
                        </tr>
                        <tr class="border-b border-solid border-slate-200">
                            <td
                                class="border-r border-solid border-white pl-4 pr-8 py-4 font-semibold text-sm text-left"
                                >Critical Thought</td
                            >
                            <td><i class="fa-solid fa-xmark text-slate-500" /></td>
                            <td><i class="fa-solid fa-check text-slate-500" /></td>
                            <td><i class="fa-solid fa-check text-slate-500" /></td>
                            <td><i class="fa-solid fa-check text-green-500 text-lg" /></td>
                        </tr>
                        <tr class="border-b border-solid border-slate-200">
                            <td
                                class="border-r border-solid border-white pl-4 pr-8 py-4 font-semibold text-sm text-left"
                                >Interpersonal Skills</td
                            >
                            <td><i class="fa-solid fa-check text-slate-500" /></td>
                            <td><i class="fa-solid fa-check text-slate-500" /></td>
                            <td><i class="fa-solid fa-xmark text-slate-500" /></td>
                            <td><i class="fa-solid fa-check text-green-500 text-lg" /></td>
                        </tr>
                         <tr class="border-b border-solid border-slate-200">
                            <td
                                class="border-r border-solid border-white pl-4 pr-8 py-4 font-semibold text-sm text-left"
                                >Programming Ability</td
                            >
                            <td><i class="fa-solid fa-check text-slate-500" /></td>
                            <td><i class="fa-solid fa-xmark text-slate-500" /></td>
                            <td><i class="fa-solid fa-check text-slate-500" /></td>
                            <td><i class="fa-solid fa-check text-green-500 text-lg" /></td>
                        </tr>
                        <tr class="border-b border-solid border-slate-200">
                            <td
                                class="border-r border-solid border-white pl-4 pr-8 py-4 font-semibold text-sm text-left"
                                >Persuasive Writing</td
                            >
                            <td><i class="fa-solid fa-check text-slate-500" /></td>
                            <td><i class="fa-solid fa-xmark text-slate-500" /></td>
                            <td><i class="fa-solid fa-check text-slate-500" /></td>
                            <td><i class="fa-solid fa-check text-green-500 text-lg" /></td>
                        </tr>
                        <tr>
                            <td
                                class="border-r border-solid border-white pl-4 pr-8 py-4 font-semibold text-sm text-left"
                                >Design Knowledge</td
                            >
                            <td><i class="fa-solid fa-check text-slate-500" /></td>
                            <td><i class="fa-solid fa-xmark text-slate-500" /></td>
                            <td><i class="fa-solid fa-check text-slate-500" /></td>
                            <td><i class="fa-solid fa-check text-green-500 text-lg" /></td>
                        </tr>
                    </tbody>
                </table>
            </div>
            <div class="mx-auto -mt-4 italic sm:hidden opacity-50">
                <p>Scroll to see more →</p>
            </div>
        </div>

    </section>
    
    <section id="skills" class="py-20 lg:py-32 flex flex-col gap-16">
        <div class="flex flex-col gap-2 text-center">
            <h6 class="text-large sm:text-xl md:text-2xl">
                My technical and professional expertise.
            </h6>
            <h3 class="font-semibold text-3xl sm:text-4xl md:text-5xl">
                My <span class="poppins text-violet-400">Skills</span>
            </h3>
        </div>
        <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 xl:grid-cols-5 gap-12 lg:gap-10">
            {#each skills as skill}
                <Step step={skill} />
            {/each}
        </div>
    </section>

    <section id="certifications" class="py-20 lg:py-32 flex flex-col gap-16">
        <div class="flex flex-col gap-2 text-center">
            <h6 class="text-large sm:text-xl md:text-2xl">
                Certified by the best.
            </h6>
            <h3 class="font-semibold text-3xl sm:text-4xl md:text-5xl">
                My <span class="poppins text-violet-400">Certifications</span>
            </h3>
        </div>
        <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-12 lg:gap-10">
            {#each certifications as cert}
                <Step step={cert} />
            {/each}
        </div>
    </section>

    <section id="testimonials" class="py-20 lg:py-32 flex flex-col gap-20">
  <div class="flex flex-col gap-4 text-center mb-10">
    <h6 class="text-large sm:text-xl md:text-2xl">
      What others say about me.
    </h6>
    <h3 class="font-semibold text-3xl sm:text-4xl md:text-5xl">
      <span class="poppins text-violet-400">Testimonials</span>
    </h3>
  </div>

  <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-10">
    {#each testimonials as test}
      <Step step={test} class="p-6 flex flex-col items-center gap-4 rounded-xl bg-slate-900 shadow-lg">
        <svelte:fragment slot="image">
          <img 
            src={test.image} 
            alt={test.name} 
            class="w-20 h-20 rounded-full border-4 border-slate-900" 
          />
        </svelte:fragment>
      </Step>
    {/each}
  </div>
  <a href="https://github.com/dikshant1602" target="_blank" rel="noopener noreferrer" class="mx-auto mt-4 px-6 py-3 rounded-md border border-solid border-white flex items-center gap-3 hover:border-violet-700 hover:bg-violet-900/20 duration-200">
            <i class="fa-brands fa-linkedin"></i>
            <p>Read More Testimonials on linkedin</p>
        </a>
</section>
</main>