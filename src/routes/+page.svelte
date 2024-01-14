<script>

    import Nav from "$lib/nav.svelte";

</script>

<main>
    <!-- banner -->
    <section id="banner" class="h-screen w-screen grid place-content-center text-center">
        <div class="">
            <h2 class="font-semibold text-primary-500 text-6xl">Hi, I'm Elijah</h2>
            <h3 class="font-bold text-7xl">I make Web Applications</h3>
        </div>
    </section>

    <Nav/>

    <!-- service cards -->
    <section id="service-cards" class="py-12">
        <div class="container mx-auto px-2">
            <header class="section-header">
                <h2>What I Do.</h2>
            </header>
            <div class="grid gap-4 md:grid-cols-3">
                <article class="home-card">
                    <h3 class="title">UI Development</h3>
                    <p class="lead">
                        Crafting captivating interfaces that blend creativity and cutting-edge technologies, I transform ideas into visually stunning user experiences that leave a lasting impact.
                    </p>
                    <a href="./"><i class="fas fa-eye"></i> Know More</a>
                </article>
                <article class="home-card highlight">
                    <h3 class="title">Backend Development</h3>
                    <p class="lead">
                        With expertise in Django and SvelteKit, I engineer robust back-end systems that power seamless functionality, ensuring your applications are both visually impressive and technically solid.
                    </p>
                    <a href="./"><i class="fas fa-eye"></i> Know More</a>
                </article>
                <article class="home-card">
                    <h3 class="title">Web Deployment</h3>
                    <p class="lead">
                        From integration to performance optimization, I handle the entire deployment process, ensuring your web applications are securely and efficiently launched for a global audience.
                    </p>
                    <a href="./"><i class="fas fa-eye"></i> Know More</a>
                </article>
            </div>
        </div>
    </section>
    <!-- skills -->
    <section id="skills" class="py-12">
        <div class="container mx-auto px-2">
            <div class="flex flex-wrap justify-center gap-8">
                <img src="img/skills/js-logo.png" alt="" class="h-8">
                <img src="img/skills/ts-logo.png" alt="" class="h-8">
                <img src="img/skills/sass-logo.png" alt="" class="h-8">
                <img src="img/skills/tailwind-css.png" alt="" class="h-8">
                <img src="img/skills/mysql-logo.png" alt="" class="h-8">
                <img src="img/skills/python-logo.png" alt="" class="h-8">
                <img src="img/skills/django-logo.png" alt="" class="h-8">
            </div>
        </div>
    </section>
    <!-- featured projects -->
    <section id="featured-projects" class="py-12">
        <div class="container mx-auto px-2">
            <header class="section-header">
                <h2>My Projects.</h2>
            </header>
            <div class="grid gap-8 sm:grid-cols-2 lg:grid-cols-3">
                
                <article class="project-card">
                    <figure class="img-control">
                        <img class="img-fluid" src="" alt="">
                    </figure>
                    <div class="info">
                        <h3>Title</h3>
                        <a href="/"><i class="fas fa-eye"></i> Know
                            more</a>
                    </div>
                </article>
                    
            </div>
        </div>
    </section>
</main>

<style lang="postcss">
</style>
