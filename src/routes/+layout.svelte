<script lang="ts">
    import '../app.css'
    import Footer from '../lib/components/Footer.svelte'
    import Header from '../lib/components/Header.svelte'
</script>

<Header/>

<main class="bg-slate-800 text-white font-mono">
    <slot />
</main>

<Footer/>
<style>
</style>
