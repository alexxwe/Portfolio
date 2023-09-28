<script lang="ts">
    import { onMount } from 'svelte'

    let isDarkMode = false
    let isExpanded = false

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

    function dropdown() {
        isExpanded = !isExpanded
    }
    
</script>

<div class="my-2 mx-4 flex items-center justify-between text-2xl font-bold sm:text-4xl">
    <div class="relative z-10">
        <button class="bi bi-file-earmark-person hover:bg-blue-500 rounded-md p-1" on:click={dropdown}></button>
        {#if isExpanded}
        <div class="absolute shadow-lg rounded bg-indigo-800 m-1 text-2xl p-1 w-16 flex-col mx-auto flex items-center ">
            <a href="/pdf/CV_Alex_esp.pdf" target="_blank">
                <button class="rounded m-1 bg-violet-400 w-12">ESP</button>
            </a>
                <a href="/pdf/CV_Alex_en.pdf" target="_blank">
                <button class="rounded m-1 bg-violet-400 w-12">EN</button>
            </a>

        </div>
        {/if}
    </div>


    <!-- svelte-ignore a11y-click-events-have-key-events -->
    <button
        ><img
            class=" rounded-full {isDarkMode ? 'bg-blue-700 hover:bg-blue-800' : 'bg-blue-600 hover:bg-blue-500'}  moon h-6 cursor-pointer p-1 sm:h-10"
            src={isDarkMode ? '/images/svg/moon.svg' : '/images/svg/sun.svg'}
            alt=""
            on:click={toggleDarkMode}
        /></button
    >

    <h1 class="flex justify-center text-2xl sm:text-4xl">Alex Paz</h1>

    <!-- svelte-ignore a11y-click-events-have-key-events -->
    <div class="toggle-button" on:click={toggleDarkMode}>
        <div class="slider {isDarkMode ? 'bg-black' : 'bg-white'}" style="transform: translateX({isDarkMode ? '100%' : '0%'});" />
    </div>
    <a href="https://github.com/alexxwe" rel="noreferrer" target="_blank"><i class="bi bi-github"/></a>
</div>

<style>
    .toggle-button {
        position: relative;
        width: 60px;
        height: 30px;
        background-color: grey;
        border-radius: 15px;
        cursor: pointer;
    }

    .slider {
        position: absolute;
        width: 50%;
        height: 100%;
        border-radius: 50%;
        transition: 0.5s ease;
    }

    @media (max-width: 639px) {
        .toggle-button {
            position: relative;
            width: 30px;
            height: 20px;
            background-color: grey;
            border-radius: 15px;
            cursor: pointer;
        }

        .slider {
            position: absolute;
            width: 50%;
            height: 100%;
            border-radius: 50%;
            transition: 0.5s ease;
        }
    }
</style>
