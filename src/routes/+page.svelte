<script lang="ts">
    import Contact from '$lib/components/Contact.svelte'
    import MouseMove from '../lib/components/mouseMove.svelte'

    const IMAGES = {
        HTML: '/images/skills/HTML.svg',
        CSS: '/images/skills/CSS.svg',
        JS: '/images/skills/javascript.svg',
        GIT: '/images/skills/Git.svg',
        TAILWINDCSS: '/images/skills/tailwindcss.svg',
        NPM: '/images/skills/npm.svg',
        SVELTE: '/images/skills/Svelte.png',
        VSCODE: '/images/skills/vscode.svg',
        GITHUB: '/images/skills/github.svg',
        NODEJS: '/images/skills/node.webp',
        NESTJS: '/images/skills/nestJS.png',
        NEXTJSLOGO: '/images/skills/nextJSlogo.svg',
        NEXTJS: '/images/skills/nextJS.svg',
        REACT: '/images/skills/react.svg',
        SASS: '/images/skills/sass.webp',
        TYPESCRIPT: '/images/skills/typescript.webp',
        VITE: '/images/skills/vite.svg',
        JEST: '/images/skills/jest.svg',
    }
</script>

<div class="senTop" />
<div id="Index" class="container mx-auto max-w-7xl xl:h-screen flex items-center justify-center">
    <div class="flex flex-col items-center lg:flex-row">
        <div class="md:p-14">
            <img src="/images/svg/undraw_digital_nomad_re_w8uy.svg" class="animate__animated animate__fadeInLeft animate__slow 2s h-32 lg:h-full" alt="" />
        </div>
        <div class="container col-span-3 flex justify-center md:col-span-2">
            <div class="card bg-slate-800">
                <h1 class="z-10 text-2xl md:text-6xl">
                    <p class="animate__animated animate__fadeInDownBig text-white">Welcome</p>
                    <p class="animate__animated animate__jackInTheBox animate__delay-1s transition duration-75 text-white">
                        I am <span class="text-indigo-600"> Alex</span>
                    </p>
                    <p class="animate__animated animate__fadeInUpBig animate__slow 500ms text-white">Software Developer</p>
                </h1>
            </div>
        </div>
    </div>
</div>

<div class="container mx-auto text-2xl m-10">
    <div class="flex flex-col md:flex-row justify-between items-center max-w-4xl xl:mx-auto md:gap-4">
        <a href="#Index" class="bg-indigo-400 dark:bg-indigo-500/70 px-2 py-1 rounded-lg hover:bg-indigo-500 dark:hover:bg-indigo-300 my-2 w-32 text-center"
            >Index</a
        >
        <a href="#Skills" class="bg-indigo-400 dark:bg-indigo-500/70 px-2 py-1 rounded-lg hover:bg-indigo-500 dark:hover:bg-indigo-300 my-2 w-32 text-center"
            >Skills</a
        >
        <a href="#About" class="bg-indigo-400 dark:bg-indigo-500/70 px-2 py-1 rounded-lg hover:bg-indigo-500 dark:hover:bg-indigo-300 my-2 w-32 text-center"
            >About</a
        >
        <a href="#Projects" class="bg-indigo-400 dark:bg-indigo-500/70 px-2 py-1 rounded-lg hover:bg-indigo-500 dark:hover:bg-indigo-300 my-2 w-32 text-center"
            >Projects</a
        >
        <a
            href="#Contributions"
            class="bg-indigo-400 dark:bg-indigo-500/70 px-2 py-1 rounded-lg hover:bg-indigo-500 dark:hover:bg-indigo-300 my-2 w-42 text-center">Contributions</a
        >
        <a href="#Me" class="bg-indigo-400 dark:bg-indigo-500/70 px-2 py-1 rounded-lg hover:bg-indigo-500 dark:hover:bg-indigo-300 my-2 w-32 text-center">Me</a>
        <a href="#Contact" class="bg-indigo-400 dark:bg-indigo-500/70 px-2 py-1 rounded-lg hover:bg-indigo-500 dark:hover:bg-indigo-300 my-2 w-32 text-center"
            >Contact</a
        >
    </div>
</div>

<div id="Skills" class="container mx-auto max-w-7xl p-4">
    <h2 class="my-4 text-center text-2xl sm:text-3xl">Technologies/Skills</h2>
    <hr class="mx-auto h-1 rounded border-0 bg-black dark:bg-white" />
    <div class="grid grid-cols-2 md:flex md:flex-col">
        <div class="flex flex-col items-center">
            <h1 class="mt-10 text-center text-xl sm:text-2xl">Web<br> Development</h1>
            <div
                class="m-4 flex flex-col items-center md:flex-row md:justify-center gap-10 rounded-full bg-slate-500 px-3 py-5 md:px-10 md:py-3 text-center text-xs"
            >
                <div class="hover:scale-125">
                    <img src={IMAGES.HTML} alt="HTML logo" class="animate__animated animate__zoomInLeft animate__slow" />
                    <i>HTML</i>
                </div>
                <div class="hover:scale-125">
                    <img src={IMAGES.CSS} alt="CSS logo" class="animate__animated animate__zoomInLeft animate__slow" />
                    <i>CSS</i>
                </div>
                <div class="hover:scale-125">
                    <img src={IMAGES.JS} alt="JavaScript logo" class="animate__animated animate__zoomInLeft animate__slow" />
                    <i>JS</i>
                </div>
                <div class="hover:scale-125">
                    <img src={IMAGES.TYPESCRIPT} alt="TypeScript logo" class=" animate__animated animate__zoomInLeft animate__slow w-11" />
                    <i>TS</i>
                </div>

                <div class="hover:scale-125">
                    <img class="animate__animated animate__zoomInRight animate__slow w-11" src={IMAGES.SVELTE} alt="Svelte logo" />
                    <i>Svelte</i>
                </div>
                <div class="hover:scale-125">
                    <img src={IMAGES.REACT} alt="React logo" class="animate__animated animate__zoomInRight animate__slow h-11" />
                    <i>React</i>
                </div>
                <div class="hover:scale-125">
                    <img src={IMAGES.TAILWINDCSS} alt="TailwindCSS logo" class="mx-auto animate__animated animate__zoomInRight animate__slow w-11" />
                    <i>TailwindCSS</i>
                </div>
                <div class="hover:scale-125">
                    <img src={IMAGES.SASS} alt="SASS logo" class="animate__animated animate__zoomInRight animate__slow h-11" />
                    <i>SASS</i>
                </div>
            </div>
        </div>
        <div>
            <div class="flex flex-col items-center">
                <h1 class="mt-10 text-center text-xl sm:text-2xl">Tools and Environment</h1>
                <div
                    class="m-4 mb-8 flex flex-col items-center md:flex-row md:justify-center gap-10 rounded-full bg-slate-500 px-3 py-6 md:px-10 md:py-3 text-center text-xs"
                >
                    <div class="hover:scale-125">
                        <img src={IMAGES.GIT} alt="Git logo" class="animate__animated animate__zoomInLeft animate__slow" />
                        <i>Git</i>
                    </div>

                    <div class="hover:scale-125">
                        <img src={IMAGES.NPM} alt="NPM logo" class="animate__animated animate__zoomInLeft animate__slow" />
                        <i>NPM</i>
                    </div>
                    <div class="hover:scale-125">
                        <img src={IMAGES.VSCODE} alt="VSCode logo" class="animate__animated animate__zoomInLeft animate__slow w-11" />
                        <i>VSCode</i>
                    </div>
                    <div class="hover:scale-125">
                        <img src={IMAGES.GITHUB} alt="GitHub logo" class="animate__animated animate__zoomInUp animate__slow w-11" />
                        <i>GitHub</i>
                    </div>
                    <div class="hover:scale-125">
                        <img src={IMAGES.NODEJS} alt="NodeJS logo" class="animate__animated animate__zoomInRight animate__slow h-11" />
                        <i>NodeJS</i>
                    </div>
                    <div class="hover:scale-125">
                        <img src={IMAGES.VITE} alt="Vite logo" class="animate__animated animate__zoomInRight animate__slow h-11" />
                        <i>Vite</i>
                    </div>
                    <div class="hover:scale-125">
                        <img src={IMAGES.JEST} alt="Jest logo" class="animate__animated animate__zoomInRight animate__slow h-11" />
                        <i>Jest</i>
                    </div>
                </div>
            </div>
        </div>
    </div>

    <hr class="mx-auto mt-6 h-1 rounded border-0 bg-black dark:bg-white" />
</div>
<div class="xl:h-screen">
    <div id="About" class="container mx-auto max-w-7xl grid grid-cols-3 p-4 text-center sm:text-start">
        <h2 class="my-4 text-center text-4xl underline col-span-3">About me:</h2>
        <!-- <div>
        <button class="rounded-full bg-indigo-600 px-2 text-xl" on:click={}>ES|EN</button>
    </div> -->
        <p class="text-lg col-span-3 lg:col-span-2 lg:text-2xl">
            Hi, I'm Alex, a <b>software developer</b> who's had a background as a <b>telecommunications technician</b>. <br /> <br />
            I'm a dedicated computer science student with a good work ethic and a burning passion for constantly improving my skills. <br />
            <br />
            What sets me apart is my commitment to achieving my goals.<br /><br />
            I enjoy working as a team, firmly believing in the importance of collaboration to achieve innovative and efficient solutions in software development.<br
            />
        </p>
        <div class="pt-10 lg:p-1 col-span-3 flex justify-center items-center lg:col-span-1">
            <img
                src="/images/alexSquare.jpg"
                alt=""
                class="rounded-full shadow-lg shadow-indigo-600 hover:shadow-xl hover:shadow-indigo-600 h-40 xl:h-90 lg:h-80 md:h-60"
            />
        </div>
    </div>
</div>

<div id="Projects" class="container mx-auto max-w-7xl p-4 xl:h-screen">
    <h2 class="my-4 text-center text-3xl">Projects</h2>
    <hr class="mx-auto h-1 rounded border-0 bg-black dark:bg-white" />
    <div class="m-4 flex justify-center">
        <section class="lg:grid lg:grid-cols-3 flex flex-col">
            <article class="flex-grow">
                <a
                    class="m-4 grid h-auto max-w-sm justify-center rounded-lg bg-indigo-500/70 p-4 shadow hover:shadow-lg hover:shadow-indigo-500 dark:hover:shadow-gray-300"
                    href="https://pokewe.vercel.app/"
                    target="_blank"
                    rel="noreferer noreferrer"
                >
                    <h1 class="flex justify-center text-4xl">PokeApi</h1>
                    <hr class="m-2 h-0.5 rounded bg-white" />

                    <img class="flex w-auto h-80 mx-auto rounded-3xl p-4" src="https://www.henryhiles.com/images/pokeApiThumb.svg" alt="PokeAPI" />
                    <p class="mt-2 text-center">Collect data and features of all Pokémon. Gotta catch'em all. <br />Made with the PokeAPI</p>
                    <div class="flex mx-auto gap-4">
                        <img class="mt-4 w-6 mx-auto" src={IMAGES.SVELTE} alt="Svelte" title="Svelte" />
                        <img class="mt-4 w-6 mx-auto" src={IMAGES.TYPESCRIPT} alt="TypeScript" title="TypeScript" />
                        <img class="mt-4 w-6 mx-auto" src={IMAGES.JS} alt="JavaScript" title="JavaScript" />
                        <img class="mt-4 w-6 mx-auto" src={IMAGES.HTML} alt="HTML" title="HTML" />
                        <img class="mt-4 w-6 mx-auto" src={IMAGES.CSS} alt="CSS" title="CSS" />
                    </div>
                </a>
            </article>

            <article class="flex-grow">
                <a
                    class="m-4 grid h-auto max-w-sm justify-center rounded-lg bg-indigo-500/70 p-4 shadow hover:shadow-lg hover:shadow-indigo-500 dark:hover:shadow-gray-300"
                    href="https://storwe.vercel.app/"
                    target="_blank"
                    rel="noreferer noreferrer"
                >
                    <h1 class="flex justify-center text-4xl">StorWe</h1>
                    <hr class="m-2 h-0.5 rounded bg-white" />

                    <img class="flex w-auto h-80 mx-auto p-6" src="https://fakestoreapi.com/icons/logo.png" alt="StoreAPI" />
                    <!-- src="https://www.definicionabc.com/wp-content/uploads/tecnologia/App-Store.jpg" -->
                    <p class="mt-2 text-center">Efficient and intuitive e-commerce website prototype. <br />Made with the StoreAPI</p>
                    <div class="flex mx-auto gap-4">
                        <img class="mt-4 w-6 mx-auto" src={IMAGES.SVELTE} alt="Svelte" title="Svelte" />
                        <img class="mt-4 w-6 mx-auto" src={IMAGES.TYPESCRIPT} alt="TypeScript" title="TypeScript" />
                        <img class="mt-4 w-6 mx-auto" src={IMAGES.JS} alt="JavaScript" title="JavaScript" />
                        <img class="mt-4 w-6 mx-auto" src={IMAGES.HTML} alt="HTML" title="HTML" />
                        <img class="mt-4 w-6 mx-auto" src={IMAGES.CSS} alt="CSS" title="CSS" />
                    </div>
                </a>
            </article>

            <article class="flex-grow">
                <a
                    class="m-4 grid h-auto max-w-sm justify-center rounded-lg bg-indigo-500/70 p-4 shadow hover:shadow-lg hover:shadow-indigo-500 dark:hover:shadow-gray-300"
                    href="https://dummywe.vercel.app/"
                    target="_blank"
                    rel="noreferer noreferrer"
                >
                    <h1 class="flex justify-center text-4xl">DummyApi</h1>
                    <hr class="m-2 h-0.5 rounded bg-white" />

                    <img class="flex w-auto h-80 mx-auto p-2" src="https://fakestoreapi.com/icons/intro.svg" alt="DummyAPI" />

                    <p class="mt-2 text-center">Bigger e-commerce website, this time with more products. <br />Made with the DummyAPI</p>
                    <div class="flex mx-auto gap-4">
                        <img class="mt-4 w-6 mx-auto" src={IMAGES.SVELTE} alt="Svelte" title="Svelte" />
                        <img class="mt-4 w-6 mx-auto" src={IMAGES.TYPESCRIPT} alt="TypeScript" title="TypeScript" />
                        <img class="mt-4 w-6 mx-auto" src={IMAGES.JS} alt="JavaScript" title="JavaScript" />
                        <img class="mt-4 w-6 mx-auto" src={IMAGES.HTML} alt="HTML" title="HTML" />
                        <img class="mt-4 w-6 mx-auto" src={IMAGES.CSS} alt="CSS" title="CSS" />
                    </div>
                </a>
            </article>
        </section>
    </div>

    <hr class="mx-auto h-1 rounded border-0 bg-black dark:bg-white" />
</div>

<div id="Contributions" class="container mx-auto max-w-7xl p-4 xl:h-screen">
    <h2 class="my-4 text-center text-3xl">Contributions</h2>
    <hr class="mx-auto h-1 rounded border-0 bg-black dark:bg-white" />
    <div class="m-4 flex justify-center">
        <section class="lg:grid lg:grid-cols-2 flex flex-col">
            <article class="flex-grow">
                <a
                    class="m-4 grid h-auto max-w-sm justify-center rounded-lg bg-indigo-500/70 p-4 shadow hover:shadow-lg hover:shadow-indigo-500 dark:hover:shadow-gray-300"
                    href="https://hexastats.vercel.app/"
                    target="_blank"
                    rel="noreferer noreferrer"
                >
                    <h1 class="flex justify-center text-4xl">Hexastats</h1>
                    <hr class="m-2 h-0.5 rounded bg-white" />

                    <img class="flex w-auto h-80 mx-auto rounded-3xl p-2" src="./images/hexastats.svg" alt="Hexastats" />
                    <p class="mt-2 text-center">League of Legends stats visualization tool.<br /></p>
                    <div class="flex mx-auto gap-4">
                        <img class="mt-4 w-6 mx-auto" src={IMAGES.SVELTE} alt="Svelte" title="Svelte" />
                        <img class="mt-4 w-6 mx-auto" src={IMAGES.TYPESCRIPT} alt="TypeScript" title="TypeScript" />
                        <img class="mt-4 w-6 mx-auto" src={IMAGES.NEXTJSLOGO} alt="NextJS" title="NextJS" />
                    </div>
                </a>
            </article>

            <article class="flex-grow">
                <a
                    class="m-4 grid h-auto max-w-sm justify-center rounded-lg bg-indigo-500/70 p-4 shadow hover:shadow-lg hover:shadow-indigo-500 dark:hover:shadow-gray-300"
                    href="https://hexakill.vercel.app/"
                    target="_blank"
                    rel="noreferer noreferrer"
                >
                    <h1 class="flex justify-center text-4xl">Hexakill</h1>
                    <hr class="m-2 h-0.5 rounded bg-white" />

                    <img class="flex w-auto h-80 mx-auto rounded-3xl p-8" src="./images/hexakill.gif" alt="hexakill" />
                    <p class="mt-2 text-center">Turn Based RPG game<br />with 3 different Characters</p>
                    <div class="flex mx-auto gap-4">
                        <img class="mt-4 w-6 mx-auto" src={IMAGES.SVELTE} alt="Svelte" title="Svelte" />
                        <img class="mt-4 w-6 mx-auto" src={IMAGES.TYPESCRIPT} alt="TypeScript" title="TypeScript" />
                        <img class="mt-4 w-6 mx-auto" src={IMAGES.JS} alt="JavaScript" title="JavaScript" />
                        <img class="mt-4 w-6 mx-auto" src={IMAGES.HTML} alt="HTML" title="HTML" />
                        <img class="mt-4 w-6 mx-auto" src={IMAGES.CSS} alt="CSS" title="CSS" />
                    </div>
                </a>
            </article>
        </section>
    </div>
    <hr class="mx-auto h-1 rounded border-0 bg-black dark:bg-white" />
</div>

<div id="Me">
    <MouseMove />
</div>

<div id="Contact" class="container mx-auto max-w-7xl mt-20 p-4">
    <h2 class="my-4 text-center text-3xl underline">Contact me:</h2>
    <hr class="mx-auto h-1 rounded border-0 bg-black dark:bg-white" />
    <Contact />
    <div class="flex justify-center mt-10">
        <img src="/images/svg/undraw_working_re_ddwy.svg" alt="" />
    </div>
</div>
<div class="senBot" />

<style>
    .senTop {
        --size: 50px;
        --p: 25px;
        --R: 55.9px /*sqrt(var(--size)*var(--size) + var(--p)*var(--p))*/;

        height: 100px;

        mask:
            radial-gradient(var(--R) at 50% calc(100% - (var(--size) + var(--p))), blue 99%, #0000 101%) calc(50% - 2 * var(--size)) 0 / calc(4 * var(--size))
                100%,
            radial-gradient(var(--R) at 50% calc(100% + var(--p)), #0000 99%, red 101%) 50% calc(100% - var(--size)) / calc(4 * var(--size)) 100% repeat-x;
        background: linear-gradient(90deg, rgb(60, 60, 216), rgb(64, 51, 153), rgb(42, 89, 245));
        border: none;
    }
    .senBot {
        --size: 50px;
        --p: 25px;
        --R: 55.9px; /* sqrt(var(--size)*var(--size) + var(--p)*var(--p)) */

        height: 100px;

        mask:
            radial-gradient(var(--R) at 50% calc(var(--size) + var(--p)), blue 99%, #0000 101%) calc(50% - 2 * var(--size)) 0 / calc(4 * var(--size)) 100%,
            radial-gradient(var(--R) at 50% calc(-1 * var(--p)), #0000 99%, red 101%) 50% var(--size) / calc(4 * var(--size)) 100% repeat-x;
        background: linear-gradient(90deg, rgb(60, 60, 216), rgb(64, 51, 153), rgb(42, 89, 245));
        border: none;
    }

    @keyframes rotate {
        0% {
            transform: rotate(0deg);
        }
        100% {
            transform: rotate(360deg);
        }
    }
    .card {
        position: relative;
        height: 30rem;
        width: 40rem;
        display: flex;
        justify-content: center;
        align-items: center;
        text-align: center;
        overflow: hidden;
        margin: 50px;
        border-radius: 30px;
        /* border-radius: 45% 45%; */
    }
    .card::before {
        content: '';
        height: 85rem;
        width: 15rem;
        background: linear-gradient(90deg, rgb(94, 94, 228), rgb(64, 51, 153), rgb(42, 89, 245));
        position: absolute;
        animation: rotate 5s linear infinite;
        right: 40%;
    }

    .card::after {
        content: '';
        height: 29rem;
        width: 39rem;
        background: rgb(30, 41, 59);
        /* background: rgb(34, 39, 42); */
        position: absolute;
        z-index: 2;
        border-radius: 30px;
        /* border-radius: 45% 45%; */
    }

    @media (max-width: 770px) {
        .card {
            height: 10rem;
            width: 17rem;
        }
        .card::before {
            height: 25rem;
            width: 4rem;
        }
        .card::after {
            height: 9.5rem;
            width: 16.5rem;
        }
    }

    @media (max-width: 400px) {
        .card {
            height: 9rem;
            width: 10rem;
        }
        .card::before {
            height: 25rem;
            width: 4rem;
        }
        .card::after {
            height: 8.5rem;
            width: 9.5rem;
        }
    }
</style>
