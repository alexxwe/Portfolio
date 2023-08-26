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

<header class="my-2 mx-4 flex items-center justify-between font-bold text-2xl sm:text-4xl">
    <a href="https://www.google.com/" rel="noreferrer" target="_blank"><i class="bi bi-file-earmark-person"></a>

    <!-- svelte-ignore a11y-click-events-have-key-events -->
    <button><img class="moon h-6 sm:h-10 cursor-pointer" src={isDarkMode ? '/images/svg/moon.svg' : '/images/svg/sun.svg'} alt="" on:click={toggleDarkMode} /></button>

    <h1 class="flex justify-center text-2xl sm:text-4xl">Alex Paz</h1>

    <!-- svelte-ignore a11y-click-events-have-key-events -->
    <div class="toggle-button" on:click={toggleDarkMode}>
        <div class="slider {isDarkMode ? 'bg-black' : 'bg-white'}" style="transform: translateX({isDarkMode ? '100%' : '0%'});" />
    </div>
    <a href="https://github.com/alexxwe" rel="noreferrer" target="_blank"><i class="bi bi-github"></a>
</header>

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
