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
        REACT: '/images/skills/react.svg',
        SASS: '/images/skills/sass.webp',
        TYPESCRIPT: '/images/skills/typescript.webp',
    }
</script>

<div class="senTop" />
<div>
    <div class="flex flex-col items-center lg:flex-row">
        <div class="md:p-14">
            <img src="/images/svg/undraw_digital_nomad_re_w8uy.svg" class="animate__animated animate__fadeInLeft animate__slow 2s h-32 lg:h-full" alt="" />
        </div>
        <div class="container col-span-3 flex justify-center md:col-span-2 ">
            <div class="card bg-slate-800">
                <h1 class="z-10 text-2xl md:text-6xl">
                    <p class="animate__animated animate__fadeInDownBig">Welcome</p>
                    <p class="animate__animated animate__jackInTheBox animate__delay-1s transition duration-75">
                        I am <span class="text-indigo-600"> Alex</span>,
                    </p>
                    <p class="animate__animated animate__fadeInUpBig animate__slow 500ms">Software Developer</p>
                </h1>
            </div>
        </div>
    </div>
</div>

<div class="container mx-auto p-4">
    <h2 class="my-4 text-center text-3xl">Technologies/Skills</h2>
    <hr class="mx-auto h-1 rounded border-0 bg-white" />
    <div class="grid grid-cols-2 md:flex md:flex-col">
        <div class="flex flex-col items-center">
            <h1 class="mt-10 text-center text-2xl">Web Development</h1>
            <div class="m-4 flex flex-col items-center md:flex-row md:justify-center gap-10 rounded-full bg-slate-500 px-2 py-5 md:px-10 md:py-2 text-center text-xs">
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
                    <img src={IMAGES.SASS} alt="SASS logo" class="animate__animated animate__zoomInRight animate__slow h-11" />
                    <i>SASS</i>
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
                    <img src={IMAGES.TAILWINDCSS} alt="TailwindCSS logo" class="animate__animated animate__zoomInRight animate__slow w-11" />
                    <i>TailwindCSS</i>
                </div>
            </div>
        </div>
        <div>
            <div class="flex flex-col items-center">
                <h1 class="mt-10 text-center text-2xl">Tools and Environment</h1>
                <div class="m-4 mb-8 flex flex-col items-center md:flex-row md:justify-center gap-10 rounded-full bg-slate-500 px-2 py-5 md:px-10 md:py-2 text-center text-xs">
                    <div class="hover:scale-125">
                        <img src={IMAGES.GIT} alt="Git logo" class="animate__animated animate__zoomInLeft animate__slow" />
                        <i>Git</i>
                    </div>

                    <div class="hover:scale-125">
                        <img src={IMAGES.NPM} alt="NPM logo" class="animate__animated animate__zoomInLeft animate__slow" />
                        <i>NPM</i>
                    </div>
                    <div class="hover:scale-125">
                        <img src={IMAGES.VSCODE} alt="VSCode logo" class="animate__animated animate__zoomInDown animate__slow w-11" />
                        <i>VSCode</i>
                    </div>
                    <div class="hover:scale-125">
                        <img src={IMAGES.GITHUB} alt="GitHub logo" class="animate__animated animate__zoomInRight animate__slow w-11" />
                        <i>GitHub</i>
                    </div>
                    <div class="hover:scale-125">
                        <img src={IMAGES.NODEJS} alt="NodeJS logo" class="animate__animated animate__zoomInRight animate__slow h-11" />
                        <i>NodeJS</i>
                    </div>
                </div>
            </div>
        </div>
    </div>

    <hr class="mx-auto h-1 rounded border-0 bg-white" />
</div>

<div class="container mx-auto grid grid-cols-3 p-4 text-center sm:text-start">
    <h2 class="my-4 text-center text-4xl underline col-span-3">About me:</h2>
    <!-- <div>
        <button class="rounded-full bg-indigo-600 px-2 text-xl" on:click={}>ES|EN</button>
    </div> -->
    <p class="text-md col-span-3 lg:col-span-2 lg:text-2xl">
        Hi, I'm Alex, a <b>software developer</b> who's had a background as a <b>telecommunications technician</b>. <br /> <br />
        I'm a dedicated computer science student with a good work ethic and a burning passion for constantly improving my skills. <br />
        <br />
        What sets me apart is my unwavering commitment to achieving my goals.<br /><br />
        I enjoy working as a team, firmly believing in the importance of collaboration to achieve innovative and efficient solutions in software development.<br
        />
    </p>
    <div class="pt-10 lg:p-1 col-span-3 flex justify-center items-center lg:col-span-1">
        <img src="/images/alexSquare.jpg" alt="" class="rounded-full shadow-lg shadow-indigo-600 hover:shadow-xl hover:shadow-indigo-600 h-32 xl:h-96 lg:h-80 md:h-60 " />
    </div>
</div>

<div class="container mx-auto p-4">
    <h2 class="my-4 text-center text-3xl">Projects</h2>
    <hr class="mx-auto h-1 rounded border-0 bg-white" />

    <div class="m-4 lg:grid lg:grid-cols-3 flex flex-col">
        <a
            class="m-4 grid h-auto max-w-sm justify-center rounded-lg bg-indigo-500/70 p-4 shadow hover:shadow-lg hover:shadow-gray-300"
            href="https://pokewe.vercel.app/"
            target="_blank"
            rel="noreferer noreferrer"
        >
            <h1 class="flex justify-center text-4xl">PokeApi</h1>
            <hr class=" m-2 h-0.5 rounded bg-white" />

            <img
                class="flex w-auto justify-center"
                src="https://images.wikidexcdn.net/mwuploads/wikidex/thumb/0/02/latest/20090125150654/Pok%C3%A9_Ball_%28Ilustraci%C3%B3n%29.png/800px-Pok%C3%A9_Ball_%28Ilustraci%C3%B3n%29.png"
                alt=""
            />
            <p class="mt-2 text-center">Select all the pokemon in my custom Pokedex. <br />Made with the PokeAPI</p>
        </a>

        <a
            class="m-4 grid h-auto max-w-sm justify-center rounded-lg bg-indigo-500/70 p-4 shadow hover:shadow-lg hover:shadow-gray-300"
            href="https://storwe.vercel.app/"
            target="_blank"
            rel="noreferer noreferrer"
        >
            <h1 class="flex justify-center text-4xl">StorWe</h1>
            <hr class=" m-2 h-0.5 rounded bg-white" />

            <img class="flex w-auto justify-center" src="https://fakestoreapi.com/icons/logo.png" alt="" />
            <!-- src="https://www.definicionabc.com/wp-content/uploads/tecnologia/App-Store.jpg" -->
            <p class="mt-2 text-center">Store simulation. <br />Made with the StoreAPI</p>
        </a>

        <a
            class="m-4 grid h-auto max-w-sm justify-center rounded-lg bg-indigo-500/70 p-4 shadow hover:shadow-lg hover:shadow-gray-300"
            href="https://dummywe.vercel.app/"
            target="_blank"
            rel="noreferer noreferrer"
        >
            <h1 class="flex justify-center text-4xl">DummyApi</h1>
            <hr class=" m-2 h-0.5 rounded bg-white" />

            <img class="flex w-auto justify-center" src="https://fakestoreapi.com/icons/intro.svg" alt="" />

            <p class="mt-2 text-center">Store simulation. <br />Made with the DummyAPI</p>
        </a>
    </div>
    <hr class="mx-auto h-1 rounded border-0 bg-white" />
</div>

<!-- <MouseMove /> -->

<div class="container mx-auto mt-20 p-4">
    <h2 class="my-4 text-center text-3xl">Contact me</h2>
    <hr class="mx-auto h-1 rounded border-0 bg-white" />
    <Contact />
    <div class="flex justify-center">
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

        mask: radial-gradient(var(--R) at 50% calc(100% - (var(--size) + var(--p))), blue 99%, #0000 101%) calc(50% - 2 * var(--size)) 0 / calc(4 * var(--size))
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

        mask: radial-gradient(var(--R) at 50% calc(var(--size) + var(--p)), blue 99%, #0000 101%) calc(50% - 2 * var(--size)) 0 / calc(4 * var(--size)) 100%,
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

    @media (max-width: 768px) {
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
</style>
