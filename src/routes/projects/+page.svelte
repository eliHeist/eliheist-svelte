<main>
    <div class="container px-2 mx-auto py-8">
        <div class="grid md:grid-cols-2 gap-8">
            
            <!-- {% for project in projects %} -->
            <article class="project-card-extended group">
                <div class="grid">
                    <div class="grid">
                        <figure class="thumbnail aspect-surface bg-grey-800 group-hover:bg-grey-700 p-4 rounded-md grid place-content-center">
                            <img src="" alt="name" class="h-full object-contain aspect-1610">
                        </figure>
                    </div>
                    <div class="pt-4">
                        <h2 class="project_title text-2xl font-semibold">Name PRJ</h2>
                        <p class="project_description font-light">
                            Description
                        </p>
                        <div class="flex flex-wrap gap-2 mt-2">
                            <!-- {% for tech in project.technologies.all %} -->
                            <span class="p-1 bg-grey-900 group-hover:bg-grey-800 text-xs rounded-md">tech name</span>
                            <!-- {% endfor %} -->
                        </div>
                        <div class="content mt-4">
                            <a href="/projects" class="text-primary-500 font-semibold uppercase">view <i class="fas fa-arrow-right text-white ml-2"></i></a>
                        </div>
                    </div>
                </div>
            </article>
                
        </div>
    </div>
</main>