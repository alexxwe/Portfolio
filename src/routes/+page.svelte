<script lang="ts">
    import MouseMove from '../lib/components/mouseMove.svelte'

    import alex from '../lib/components/public/assets/image/alexSquare.jpg'
    // import pair_programming from '../lib/components/public/assets/svg/undraw_pair_programming_re_or4x.svg'
    import digital_nomad from '../lib/components/public/assets/svg/undraw_digital_nomad_re_w8uy.svg'
    // import programming from '../lib/components/public/assets/svg/undraw_programming_re_kg9v.svg'
    import working from '../lib/components/public/assets/svg/undraw_working_re_ddwy.svg'

    import HTML from '../lib/components/public/assets/imgSkills/HTML.svg'
    import CSS from '../lib/components/public/assets/imgSkills/CSS.svg'
    import JS from '../lib/components/public/assets/imgSkills/javascript.svg'
    import GIT from '../lib/components/public/assets/imgSkills/Git.svg'
    import TAILWINDCSS from '../lib/components/public/assets/imgSkills/tailwindcss.svg'
    import NPM from '../lib/components/public/assets/imgSkills/npm.svg'
    import SVELTE from '../lib/components/public/assets/imgSkills/Svelte.png'
    import VSCODE from '../lib/components/public/assets/imgSkills/vscode.svg'
    import GITHUB from '../lib/components/public/assets/imgSkills/github.svg'
    import NODJS from '../lib/components/public/assets/imgSkills/node.webp'
    import REACT from '../lib/components/public/assets/imgSkills/react.webp'
    import SASS from '../lib/components/public/assets/imgSkills/sass.webp'
    import TYPESCRIPT from '../lib/components/public/assets/imgSkills/typescript.webp'

    
</script>
<div class="senTop"></div>
<div>
    <div class="grid grid-cols-3 items-center">
        <div class="p-14">
            <img src={digital_nomad} class="animate__animated animate__fadeInLeft h-full" alt="" />
        </div>
        <div class="conteiner flex justify-center col-span-2 ">
                <div class="card bg-zinc-800">
                <h1 class="z-10 text-6xl">
                    <p class="animate__animated animate__fadeInDownBig">Welcome</p>
                    <p class="animate__animated animate__jackInTheBox animate__delay-1s   transition duration-75">
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

    <div class="flex justify-center gap-10 ">
        <div class="m-10 flex items-center justify-center gap-10 rounded-full bg-gray-500 px-10 py-2 text-center text-xs">
            <div class="hover:scale-125">
                <img src={HTML} alt="HTML logo" class="animate__animated animate__slideInLeft animate__slow 250ms" />
                <i>HTML</i>
            </div>
            <div class="hover:scale-125">
                <img src={CSS} alt="CSS logo" class="animate__animated animate__slideInLeft animate__slow 250ms" />
                <i>CSS</i>
            </div>
            <div class="hover:scale-125">
                <img src={JS} alt="Javascript logo" class="animate__animated animate__slideInUp animate__slow 250ms" />
                <i>JS</i>
            </div>
            <div class="hover:scale-125">
                <img class="animate__animated animate__slideInDown animate__slow 250ms w-9" src={SVELTE} alt="Svelte logo" />
                <i>Svelte</i>
            </div>
            <div class="hover:scale-125">
                <img src={GIT} alt="Git logo" class="animate__animated animate__slideInDown animate__slow 250ms" />
                <i>Git</i>
            </div>
            <div class="hover:scale-125">
                <img src={TAILWINDCSS} alt="TailwindCSS logo" class="animate__animated animate__slideInUp animate__slow 250ms" />
                <i>TailwindCSS</i>
            </div>
            
            <div class="hover:scale-125">
                <img src={NPM} alt="NPM logo" class="animate__animated animate__slideInRight animate__slow 250ms" />
                <i>NPM</i>
            </div>
            <div class="hover:scale-125">
                <img src={VSCODE} alt="VSCode logo" class="animate__animated animate__slideInRight animate__slow 250ms" />
                <i>VSCode</i>
            </div>
            
        </div>
    </div>
    <hr class="mx-auto h-0.5 rounded border-0 bg-white" />
</div>

<div class="container mx-auto grid grid-cols-3 p-4">
    <h2 class="my-4 text-center text-4xl">About me:</h2>
    <hr class="mx-auto h-1 rounded border-0 bg-white" />
    <!-- <div>
        <button class="rounded-full bg-indigo-600 px-2 text-xl" on:click={}>ES|EN</button>
    </div> -->
    <p class="col-span-2 text-2xl">
        Hi, I'm Alex, a <b>software developer</b> who's had a background as a <b>telecommunications technician</b>. <br /> <br />
        I'm a dedicated computer science student with a good work ethic and a burning passion for constantly improving my skills. <br />
        <br />
        What sets me apart is my unwavering commitment to achieving my goals.<br /><br />
        I enjoy working as a team, firmly believing in the importance of collaboration to achieve innovative and efficient solutions in software development.<br
        />
    </p>
    <div class="p-14">
        <img src={alex} alt="" class="rounded-full shadow-lg shadow-indigo-600 hover:shadow-xl hover:shadow-indigo-600" />
    </div>
</div>

<div class="container mx-auto p-4">
    <h2 class="my-4 text-center text-3xl">Projects</h2>
    <hr class="mx-auto h-1 rounded border-0 bg-white" />

    <div class="m-4 grid grid-cols-3">
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
            <hr class="mx-auto h-1 rounded border-0 bg-white" />
            <p class="flex justify-center">Select all the pokemon in my custom Pokedex. <br />Made with the PokeAPI</p>
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
            <hr class="mx-auto h-1 rounded border-0 bg-white" />
            <p class="flex justify-center">Store simulation. <br />Made with the StoreAPI</p>
        </a>

        <a
            class="m-4 grid h-auto max-w-sm justify-center rounded-lg bg-indigo-500/70 p-4 shadow hover:shadow-lg hover:shadow-gray-300"
            href="https://storwe.vercel.app/"
            target="_blank"
            rel="noreferer noreferrer"
        >
            <h1 class="flex justify-center text-4xl">DummyApi</h1>
            <hr class=" m-2 h-0.5 rounded bg-white" />

            <img class="flex w-auto justify-center" src="https://fakestoreapi.com/icons/intro.svg" alt="" />

            <hr class="mx-auto h-1 rounded border-0 bg-white" />
            <p class="flex justify-center">Store simulation. <br />Made with the DummyAPI</p>
        </a>
    </div>
    <hr class="mx-auto h-1 rounded border-0 bg-white" />
</div>

<MouseMove />

<div class="container mx-auto mt-20 p-4">
    <h2 class="my-4 text-center text-3xl">Contact me</h2>
    <hr class="mx-auto h-1 rounded border-0 bg-white" />
    <div class="flex justify-center">
        <img src={working} alt="" />
    </div>
</div>
<div class="senBot"></div>
<style>

.senTop {
  --size: 50px;
  --p: 25px;
  --R: 55.9px /*sqrt(var(--size)*var(--size) + var(--p)*var(--p))*/;
  
  height: 100px;

  mask:
    radial-gradient(var(--R) at 50% calc(100% - (var(--size) + var(--p))),blue 99%,#0000 101%) calc(50% - 2*var(--size)) 0/calc(4*var(--size)) 100%,
    radial-gradient(var(--R) at 50% calc(100% + var(--p)),#0000 99%,red 101%) 50% calc(100% - var(--size))/calc(4*var(--size)) 100% repeat-x;
  background:linear-gradient(90deg, rgb(60, 60, 216), rgb(64, 51, 153),rgb(42, 89, 245));  
  border: none;
}
.senBot{
    --size: 50px;
  --p: 25px;
  --R: 55.9px; /* sqrt(var(--size)*var(--size) + var(--p)*var(--p)) */;

  height: 100px;

  mask:
    radial-gradient(var(--R) at 50% calc(var(--size) + var(--p)),blue 99%,#0000 101%) calc(50% - 2*var(--size)) 0/calc(4*var(--size)) 100%,
    radial-gradient(var(--R) at 50% calc(-1*var(--p)),#0000 99%,red 101%) 50% var(--size)/calc(4*var(--size)) 100% repeat-x;
    background:linear-gradient(90deg, rgb(60, 60, 216), rgb(64, 51, 153),rgb(42, 89, 245));  
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
    }
    .card::before {
        content: '';
        height: 85rem;
        width: 15rem;
        background: linear-gradient(90deg, rgb(94, 94, 228), rgb(64, 51, 153),rgb(42, 89, 245) );
        position: absolute;
        animation: rotate 3.5s linear infinite;
        right: 40%;
    }

    .card::after {
        content: '';
        height: 29rem;
        width: 39rem;
        background: rgb(40, 40, 40);
        /* background: rgb(34, 39, 42); */
        position: absolute;
        z-index: 2;
    }
</style>
