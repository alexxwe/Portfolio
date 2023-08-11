<script lang="ts">
    import MouseMove from '../lib/components/mouseMove.svelte'

    import pair_programming from '../lib/components/public/assets/svg/undraw_pair_programming_re_or4x.svg'
    import digital_nomad from '../lib/components/public/assets/svg/undraw_digital_nomad_re_w8uy.svg'
    import programming from '../lib/components/public/assets/svg/undraw_programming_re_kg9v.svg'
    import HTML from '../lib/components/public/assets/svg/HTML.svg'
    import CSS from '../lib/components/public/assets/svg/CSS.svg'
    import JS from '../lib/components/public/assets/svg/javascript.svg'
    import GIT from '../lib/components/public/assets/svg/Git.svg'
    import TAILWINDCSS from '../lib/components/public/assets/svg/tailwindcss.svg'
    import NPM from '../lib/components/public/assets/svg/npm.svg'
    import SVELTE from '../lib/components/public/assets/svg/Svelte.png'
    import VSCODE from '../lib/components/public/assets/svg/vscode.svg'
</script>

<div>
    <div class="grid grid-cols-3  items-center">
        <div class="p-14">
            <img src={digital_nomad} class="h-full opacity-100" alt="" />
        </div>
        <h1 class="flex items-center justify-center text-4xl ">
            Welcome<br />
            I am Alex,<br />
            Software Developer
        </h1>
        <div class="p-14">
            <img src={pair_programming} class="opacity-100" alt="" />
        </div>
    </div>
</div>

<div class="container mx-auto p-4">
    <h2 class="my-4 text-center text-3xl">Technologies/Skills</h2>
    <hr class="mx-auto h-1 rounded border-0 bg-white" />

    <div class="flex justify-center gap-10 ">
        <div class="m-6 flex items-center justify-center gap-10 rounded-full bg-gray-500 px-10 py-2 text-center text-xs">
            <div>
                <img src={HTML} alt="HTML logo" class="animate__animated animate__slideInLeft" />
                <i>HTML</i>
            </div>
            <div>
                <img src={CSS} alt="CSS logo" class="animate__animated animate__slideInLeft" />
                <i>CSS</i>
            </div>
            <div>
                <img src={JS} alt="Javascript logo" class="animate__animated animate__slideInUp" />
                <i>JavaScripat</i>
            </div>
            <div>
                <img src={GIT} alt="Git logo" class="animate__animated animate__slideInDown" />
                <i>Git</i>
            </div>
            <div>
                <img src={TAILWINDCSS} alt="TailwindCSS logo" class="animate__animated animate__slideInDown" />
                <i>TailwindCSS</i>
            </div>
            <div>
                <img src={NPM} alt="NPM logo" class="animate__animated animate__slideInUp" />
                <i>NPM</i>
            </div>
            <div>
                <img src={VSCODE} alt="VSCode logo" class="animate__animated animate__slideInRight" />
                <i>VSCode</i>
            </div>
            <div>
                <img class="animate__animated animate__slideInRight w-9" src={SVELTE} alt="Svelte logo" />
                <i>Svelte</i>
            </div>
        </div>
    </div>
    <hr class="mx-auto h-0.5 rounded border-0 bg-white" />
</div>

<div class="mt-30 container mx-auto grid grid-cols-3 p-4">
    <h2 class="my-4 text-center text-4xl">About me:</h2>
    <hr class="mx-auto h-1 rounded border-0 bg-white" />
    <p class="col-span-2 text-2xl">
        Hi, I'm Alex, a <b>software developer</b> and previously a <b>telecommunications technician</b>. <br />
        a<br />
        a<br />
        b
    </p>
    <div class="p-14">
        <img src={programming} alt="" />
    </div>
</div>

<div class="mt-30 container mx-auto p-4">
    <h2 class="my-4 text-center text-3xl">Projects</h2>
    <hr class="mx-auto h-1 rounded border-0 bg-white" />
    
    <div class="grid grid-cols-3 m-4">
        <div class="m-4 grid h-auto max-w-sm justify-center rounded-lg bg-indigo-500/70 p-4 shadow hover:shadow-lg hover:shadow-gray-300">
            <h1 class="flex justify-center text-4xl">PokeApi</h1>
            <hr class=" m-2 h-0.5 rounded bg-white" />

            <img
                class="flex w-auto justify-center"
                src="https://images.wikidexcdn.net/mwuploads/wikidex/thumb/0/02/latest/20090125150654/Pok%C3%A9_Ball_%28Ilustraci%C3%B3n%29.png/800px-Pok%C3%A9_Ball_%28Ilustraci%C3%B3n%29.png"
                alt=""
            />
            <hr class="mx-auto h-1 rounded border-0 bg-white" />
            <p class="flex justify-center">Select all the pokemon in my custom Pokedex. <br />Made with the PokeAPI</p>
        </div>

        <div class="m-4 grid h-auto max-w-sm justify-center rounded-lg bg-indigo-500/70 p-4 shadow hover:shadow-lg hover:shadow-gray-300">
            <h1 class="flex justify-center text-4xl">StorWe</h1>
            <hr class=" m-2 h-0.5 rounded bg-white" />

            <img class="flex w-auto justify-center" src="https://www.definicionabc.com/wp-content/uploads/tecnologia/App-Store.jpg" alt="" />

            <hr class="mx-auto h-1 rounded border-0 bg-white" />
            <p class="flex justify-center">Store simulation. <br />Made with the StoreAPI</p>
        </div>

        <div class="m-4 grid h-auto max-w-sm justify-center rounded-lg bg-indigo-500/70 p-4 shadow hover:shadow-lg hover:shadow-gray-300">
            <h1 class="flex justify-center text-4xl">DummyApi</h1>
            <hr class=" m-2 h-0.5 rounded bg-white" />

            <img class="flex w-auto justify-center" src="https://fakestoreapi.com/icons/intro.svg" alt="" />

            <hr class="mx-auto h-1 rounded border-0 bg-white" />
            <p class="flex justify-center">Store simulation. <br />Made with the DummyAPI</p>
        </div>
    </div>
    <hr class="mx-auto h-1 rounded border-0 bg-white" />
</div>

<MouseMove />

<div class="mt-30 container mx-auto p-4">
    <h2 class="my-4 text-center text-3xl">Images</h2>
    <hr class="mx-auto h-1 rounded border-0 bg-white" />
</div>
