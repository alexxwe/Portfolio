<script lang="ts">
    import '../app.css'
    import Footer from '../lib/components/Footer.svelte'
    import Header from '../lib/components/Header.svelte'
</script>

<Header/>

<main class="bg-indigo-300 dark:bg-slate-800 text-black dark:text-white  font-mono">
    <slot />
</main>

<Footer/>
<style>
</style>
