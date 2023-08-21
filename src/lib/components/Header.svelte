<script lang="ts">
    import { onMount } from 'svelte'

    let isDarkMode = false

    onMount(() => {
        const savedTheme = localStorage.getItem('theme')
        if (savedTheme === 'dark') {
            toggleDarkMode()
        }
    })

    export function toggleDarkMode() {
        isDarkMode = !isDarkMode

        if (isDarkMode) {
            document.documentElement.classList.add('dark')
            localStorage.setItem('theme', 'dark')
        } else {
            document.documentElement.classList.remove('dark')
            localStorage.setItem('theme', 'light')
        }
    }
</script>

<header class="my-2 mx-4 flex items-center justify-between font-bold">
    <a href="https://storwe.vercel.app/" rel="icon" target="_self"><i class=" bi bi-box-fill text-4xl" /><br />Store</a>
    <!-- <button class="text-3xl"> <a href="/projects">Projects</a> </button> -->
    <!-- svelte-ignore a11y-click-events-have-key-events -->
    <img class="sun h-10 cursor-pointer" src="/images/svg/moon.svg" alt="" on:click={toggleDarkMode} />
    <h1 class="flex justify-center text-4xl">Alex Paz</h1>
    <!-- <button class="text-3xl">CV?</button> -->
    <!-- svelte-ignore a11y-click-events-have-key-events -->
    <img class="moon h-10 cursor-pointer" src="/images/svg/sun.svg" alt="" on:click={toggleDarkMode} />
    <a href="https://pokeapi-alexxpf.vercel.app/" rel="noreferrer" target="_blank"><i class="bi bi-record-circle text-4xl" /><br />Poke</a>
</header>
