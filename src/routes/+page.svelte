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
<div class="mt-30 container mx-auto grid grid-cols-3 p-4">
    <h2 class="my-4 text-center text-3xl">About me</h2>
    <hr class="mx-auto h-1 rounded border-0 bg-white" />
    <p class="col-span-2">
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
    <h2 class="my-4 text-center text-3xl">Technologies/Skills</h2>
    <hr class="mx-auto h-1 rounded border-0 bg-white" />

            <div class="flex m-4 gap-10 text-xs text-center items-center justify-center bg-gray-500 rounded-full">
              <div>
                <img src={HTML} alt="HTML logo" />
                <i>HTML</i>
              </div>
              <div>
                <img src={CSS} alt="CSS logo" />
                <i>CSS</i>
              </div>
              <div>
                <img src={JS} alt="Javascript logo" />
                <i>JavaScripat</i>
              </div>
              <div>
                <img src={GIT} alt="Git logo" />
                <i>Git</i>
              </div>
              <div>
                <img src={TAILWINDCSS} alt="TailwindCSS logo" />
                <i>TailwindCSS</i>
              </div>
              <div>
                <img src={NPM} alt="NPM logo" />
                <i>NPM</i>
              </div>
              <div>
                <img src={VSCODE} alt="VSCode logo" />
                <i>VSCode</i>
              </div>
              <div>
                <img class="w-9" src={SVELTE} alt="Svelte logo" />
                <i>Svelte</i>
              </div>
            </div>
    <hr class="mx-auto h-0.5 rounded border-0 bg-white" />

</div>

<div class="mt-30 container mx-auto p-4">
    <h2 class="my-4 text-center text-3xl">Projects</h2>
    <hr class="mx-auto h-1 rounded border-0 bg-white" />
</div>

<div class="mt-30 container mx-auto p-4">
    <h2 class="my-4 text-center text-3xl">Images</h2>
    <hr class="mx-auto h-1 rounded border-0 bg-white" />
</div>

<MouseMove />
