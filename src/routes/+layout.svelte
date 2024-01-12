<script>
    import Footer from "$lib/footer.svelte";
    import Nav from "$lib/nav.svelte";
    import "../app.scss";
</script>

<div class="bg-dark text-white font-poppins  selection:bg-primary-500 selection:text-white scroll-smooth">
    <Nav/>
    <slot />
    <Footer/>
</div>