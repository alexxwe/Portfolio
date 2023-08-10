<script lang="ts">
    import '../app.css'
    import Footer from '../lib/components/Footer.svelte'
    import Header from '../lib/components/Header.svelte'
</script>

<Header/>

<main class="bg-zinc-700 text-white">
    <slot />
</main>

<Footer/>
<style>
</style>
