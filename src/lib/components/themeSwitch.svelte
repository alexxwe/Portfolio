<script lang="ts">
    import { onMount } from "svelte"

let isDarkMode = false;

onMount(() => {
    const savedTheme = localStorage.getItem('theme');
    if (savedTheme === 'dark') {
        toggleDarkMode();
    }
});

export function toggleDarkMode() {
    isDarkMode = !isDarkMode;

    if (isDarkMode) {
        document.documentElement.classList.add('dark');
        localStorage.setItem('theme', 'dark');
    } else {
        document.documentElement.classList.remove('dark');
        localStorage.setItem('theme', 'light');
    }
}
</script>

