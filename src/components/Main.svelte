<script>
    import Step from "./Step.svelte";

    let steps = [
        {
            name: "VulnScanner CLI",
            icon: "fa-solid fa-bug",
            href: "https://github.com/euphoric-habromaniac/vulnerability-scanner", // Add the actual link to the project
            description:
                "VulnScanner CLI is a lightweight Python-based command-line tool that scans for open ports, outdated server banners, missing security headers, and known vulnerabilities using public APIs. It mimics basic recon workflows used in pentesting and bug bounty hunting.",
        },
        {
            name: "SecurePaste",
            icon: "fa-solid fa-lock",
            href: "", // Add the actual link to the project
            description:
                "SecurePaste is a client-side encrypted pastebin built with Next.js and Firebase that allows users to securely share sensitive snippets with password protection, expiry timers, and self-destruct features — ensuring confidentiality even after sharing.",
        },
        {
            name: "LogWarden",
            icon: "fa-solid fa-shield-halved",
            href: "", // Add the actual link to the project
            description:
                "LogWarden is a Linux-focused log monitor that watches system auth logs for suspicious activity and automatically blocks brute-force attempts using iptables or ufw. It runs silently in the background and notifies users of repeated attacks or anomalies.",
        },
        {
            name: "ForensicBox",
            icon: "fa-solid fa-magnifying-glass",
            href: "", // Add the actual link to the project
            description:
                "ForensicBox is a digital forensics utility that extracts metadata, recovers deleted files, and analyzes recent activity on Windows and Linux machines. Built using Python and shell scripts, it simulates real-world incident response workflows in small orgs.",
        },
        {
            name: "Exploit Playground",
            icon: "fa-solid fa-skull-crossbones",
            href: "", // Add the actual link to the project
            description:
                "Exploit Playground is a collection of intentionally vulnerable C programs showcasing common security flaws like buffer overflows and format string vulnerabilities. Each binary includes a walkthrough and working exploit to demonstrate low-level attack techniques.",
        },
        {
            name: "NetShield Dashboard",
            icon: "fa-solid fa-network-wired",
            href: "", // Add the actual link to the project
            description:
                "NetShield Dashboard is a local web-based network monitoring system that identifies connected devices, runs basic scans (nmap, traceroute), and detects suspicious behavior like duplicate MACs or new intrusions — perfect for home labs and small offices.",
        },
        {
            name: "AI Malware Classifier",
            icon: "fa-solid fa-robot",
            href: "", // Add the actual link to the project
            description:
                "AI Malware Classifier is a Python-based machine learning tool that analyzes Windows executables for malicious behavior by examining static features like entropy, strings, and API imports. It uses scikit-learn to classify malware and visualize predictions.",
        },
    ];

    let benefits = [
        {
            metric: "10x",
            name: "a self taught developer",
            description:
                "I'm a self taught programmer who started with basic webdev and python, then slowly got pulled into cybersecurity with my growing facination with hackers in movies. While not a specialist in most of them, I’ve explored everything from scripting and full-stack development to reverse engineering and automation.",
        },
        {
            name: "an efficient problem solver",
            description:
                "I like to build things that arent just functional, but optimized. Whether its writting compact logic in C++, automating workflows in python, or making systems more efficient.  I focus on speed, structure, and reliability. I've worked across different layers of development, from scripting to system level code, and always try to keep performance and clarity at the core.",
        },
        {
            name: "an excellent communicator",
            description:
                "Communication is key and it's a paramount value of mine. I believe in transparency and constructive communication above all else. This helps me develop deep relationships and ensures my effectiveness and productivity in any work space with any team.",
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
            <br />
            <br />
            <br />
            <br />
            <br />
            <h2 class="font-semibold text-4xl sm:text-5xl md:text-6xl">
                Hi! I'm <span class="poppins text-violet-400">Pranjal</span> Kumar.
                <br />Student, Cybersecurity Enthusiast
                <span class="poppins text-violet-400">and Freelancer</span>
            </h2>
            <p class="text-base sm:text-lg md:text-xl">
                i <span class="text-violet-400">break systems</span> to understand them, and <span class="text-violet-400">secure them</span> so others don’t have to.
            </p>
            <a href="mailto:contact@pranjalkumar.com">
            <button
                class="blueShadow mx-auto lg:mr-auto lg:ml-0 text-base sm:text-lg md:text-xl poppins relative overflow-hidden px-6 py-3 group rounded-full bg-white text-slate-950"
            >
                <div
                    class="absolute top-0 right-full w-full h-full bg-violet-400 opacity-20 group-hover:translate-x-full z-0 duration-200" href="mailto:contact@pranjalkumar.com"></div>
                <h4 class="relative z-9">Get in touch &rarr;</h4>
            </button>
            </a>
        </div>
        <div class="relative shadow-2xl grid place-items-center max-h-[70vh]">
            {#if typeof window !== 'undefined'}
                <lottie-player
                    src="/assets/lottie.json"
                    background="transparent"
                    speed="1"
                    loop
                    autoplay
                    style="width: 100%; height: 100%; max-height: 70vh"
                ></lottie-player>
            {/if}
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
            <i class="fa-regular fa-circle-play"></i>
            <p>Watch the video</p>
        </a>
        <div class="grid grid-cols-1 lg:grid-cols-3 gap-12 lg:gap-10">
            <Step step={steps[0]}>
                <p>
                    VulnScanner CLI is a <strong class="text-violet-400">lightweight Python-based command-line tool</strong> that scans for open ports, 
                    outdated server banners, missing security headers, and known vulnerabilities using public APIs. It mimics basic recon workflows used 
                    in pentesting and bug bounty hunting.
                </p>
            </Step>
            <Step step={steps[1]}>
                <p>
                    SecurePaste is a <strong class="text-violet-400">client-side encrypted pastebin</strong> built with Next.js and Firebase that allows users to securely
                     share sensitive snippets with password protection, expiry timers, and self-destruct features; ensuring confidentiality even after sharing.
                </p>
            </Step>
            <Step step={steps[2]}>
                <p>
                    LogWarden is a <strong class="text-violet-400">Linux-focused log monitor</strong> that watches system auth logs for suspicious activity and automatically blocks brute-force attempts using iptables or ufw. It runs silently in the background and notifies users of repeated attacks or anomalies.
                </p>
            </Step>
            <Step step={steps[3]}>
                <p>
                    ForensicBox is a <strong class="text-violet-400">digital forensics utility</strong> that extracts metadata, recovers deleted files, and analyzes recent activity on Windows
                     and Linux machines. Built using Python and shell scripts, it simulates real-world incident response workflows in small orgs.
                </p>
            </Step>
            <Step step={steps[4]}>
                <p>
                    Exploit Playground is a <strong class="text-violet-400">collection of intentionally vulnerable C programs</strong> showcasing common security flaws like buffer overflows and 
                    format string vulnerabilities. Each binary includes a walkthrough and working exploit to demonstrate low-level attack techniques.
                </p>
            </Step>
            <Step step={steps[5]}>
                <p>
                    NetShield Dashboard is a <strong class="text-violet-400">local web-based network monitoring system</strong> that identifies connected devices, runs basic scans 
                    (nmap, traceroute), and detects suspicious behavior like duplicate MACs or new intrusions — perfect for home labs and small offices.
                </p>
            </Step>
            <Step step={steps[6]}>
                <p>
                    AI Malware Classifier is a <strong class="text-violet-400">Python-based machine learning tool</strong> that analyzes Windows executables for malicious behavior by 
                    examining static features like entropy, strings, and API imports. It uses scikit-learn to classify malware and visualize predictions.
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
        </div>
        <div class="mx-auto -mt-12 italic sm:hidden opacity-50">
            <p>Scroll to see more &rarr;</p>
        </div>
        <p class="mx-auto">So why not invest?</p>
    </section>
</main>