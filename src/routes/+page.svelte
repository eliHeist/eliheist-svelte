<script>
</script>

<main>
    <!-- banner -->
    <section id="banner" class="banner">
        <img src="img/laptop-banner.webp" class="banner_image" alt="" />
        <div class="banner__content">
            <h1 class="banner__title">Hi, I'm <span>Elijah</span></h1>
            <p>Specialized in full-stack Web Development</p>
        </div>
    </section>

    <section class="services">
        <div class="container">
            <div class="grid lg:grid-cols-2 gap-4">
                <div class="card">
                    <h2>Web Applications powered by Python and Django.</h2>
                </div>
                <div class="tech_list">
                    <div class="item">
                        <i class="fa-solid fa-laptop"></i>
                        <div class="grid">
                            <h3>Expertise in Python</h3>
                        </div>
                        <div class="separater"></div>
                        <p>
                            Proficient in Django and Python to build robust
                            backends.
                        </p>
                    </div>
                    <div class="item">
                        <i class="fa-solid fa-cloud"></i>
                        <div class="grid">
                            <h3>Cloud Integration</h3>
                        </div>
                        <div class="separater"></div>
                        <p>
                            Experienced with Microsoft Azure, PythonAnywhere and
                            cross application integration.
                        </p>
                    </div>
                    <div class="item">
                        <i class="fa-solid fa-database"></i>
                        <div class="grid">
                            <h3>Data Management</h3>
                        </div>
                        <div class="separater"></div>
                        <p>Experience in MySQL and PostgreSQL</p>
                    </div>
                    <div class="item">
                        <i class="fa-solid fa-shield-halved"></i>
                        <div class="grid">
                            <h3>Security Best Practices</h3>
                        </div>
                        <div class="separater"></div>
                        <p>I use a security first approach to development</p>
                    </div>
                </div>
            </div>
        </div>
    </section>
    <!-- skills -->
    <section id="skills" class="py-16">
        <div class="container mx-auto px-2">
            <div class="flex flex-wrap justify-center gap-8">
                <img src="img/skills/js-logo.png" alt="" class="h-8" />
                <img src="img/skills/ts-logo.png" alt="" class="h-8" />
                <img src="img/skills/sass-logo.png" alt="" class="h-8" />
                <img src="img/skills/tailwind-css.png" alt="" class="h-8" />
                <img src="img/skills/mysql-logo.png" alt="" class="h-8" />
                <img src="img/skills/python-logo.png" alt="" class="h-8" />
                <img src="img/skills/django-logo.png" alt="" class="h-8" />
            </div>
        </div>
    </section>
    <!-- Intuitive responsive -->
    <section class="py-20">
        <div class="intuitive_grid">
            <figure>
                <img src="img/iphone-mockup.png" alt="" class="mouse_rotate" />
            </figure>
            <div class="content">
                <div class="w-fit">
                    <h2>Intuitive and Responsive Apps</h2>
                    <p>
                        I build web applications that are easy to use, and run
                        smoothly on all devices
                    </p>
                    <img
                        src="img/boxes3.png"
                        alt=""
                        class="boxes mouse_rotate" />
                </div>
            </div>
        </div>
    </section>
    <!-- future driven -->
    <section class="future_driven">
        <div class="container">
            <div class="call_to_action">
                <h2>Get in touch.</h2>
                <p>Reach out and lets start building something great.</p>
                <ul>
                    <li>
                        <a href="https://twitter.com/eliHeist256"
                            ><i class="fa-brands fa-x-twitter"></i></a>
                    </li>
                    <li>
                        <a href="https://www.linkedin.com/in/elijahtriumph/"
                            ><i class="fa-brands fa-linkedin-in"></i></a>
                    </li>
                    <li>
                        <a href="https://www.instagram.com/eliheist/"
                            ><i class="fa-brands fa-instagram"></i></a>
                    </li>
                </ul>
            </div>
            <figure>
                <img src="img/bottom_image.webp" alt="" />
            </figure>
        </div>
    </section>
</main>

<style lang="postcss">
    .banner {
        max-height: 100svh;
        display: grid;
        align-content: end;
        position: relative;

        .banner__content {
            position: absolute;
            inset: 0;
            z-index: 2;
            display: grid;
            place-content: center;

            h1 {
                text-align: center;
                font-size: calc(2rem + 1vw);
                font-weight: 700;
                line-height: 1.2;
                color: var(--white);
            }

            p {
                max-width: 70%;
                margin: 0.5rem auto;
                text-align: center;
                color: var(--grey-100);
                font-weight: 200;
            }
        }
    }

    .services {
        background-color: var(--grey-800);
        padding: 4rem 0;

        .card {
            h2 {
                font-size: calc(2rem + 3vw);
                font-weight: 700;
                margin-bottom: 1rem;

                @media screen and (max-width: 1024px) {
                    font-size: calc(2rem + 1vw);
                }
            }
        }

        .tech_list {
            display: grid;
            align-content: center;
            gap: 1rem;
            color: var(--grey-100);
            max-width: 30rem;

            .item {
                display: grid;
                grid-template-columns: auto auto;
                grid-template-rows: auto auto;
                column-gap: 1rem;
                row-gap: 0.25rem;
                align-items: center;
                justify-content: start;
                i {
                    width: 1.5rem;
                    display: grid;
                    justify-content: center;
                    font-size: 1.25rem;
                }
                h3 {
                    font-size: 1.25rem;
                    font-weight: 600;
                }
                p {
                    font-size: 1rem;
                }
            }
        }
    }

    .intuitive_grid {
        display: grid;
        grid-template-columns: 1fr 1fr;
        gap: 4rem;
        place-items: center;

        figure img {
            max-height: 40rem;
        }

        .content {
            max-width: 30rem;
            .w-fit {
                width: 100%;
                display: grid;
                row-gap: 1rem;
            }
            h2 {
                font-size: calc(2rem + 0.5vw);
                font-weight: 700;
                margin-bottom: 1rem;
                width: fit-content;
            }
            p {
                color: var(--grey-100);
            }
            img.boxes {
                max-height: 30rem;
                margin-top: 1rem;
            }
        }
    }

    .future_driven {
        padding: 5rem 0;
        background-color: var(--grey-800);

        .container {
            display: grid;
            gap: 1rem;
            grid-template-columns: 1fr 1fr;
            align-items: center;
            @media screen and (max-width: 640px) {
                grid-template-columns: 1fr;
            }

            .call_to_action {
                color: var(--grey-100);
                h2 {
                    color: var(--white);
                    font-size: calc(2rem + 0.5vw);
                    font-weight: 700;
                    margin-bottom: 1rem;
                }

                ul {
                    display: flex;
                    gap: 1rem;
                    margin-top: 5rem;
                    li {
                        i {
                            font-size: 1.5rem;
                            color: var(--grey-100);
                        }
                    }
                }
            }
        }
    }
</style>
