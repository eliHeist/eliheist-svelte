<script lang="ts">
    import { onMount } from "svelte";

    let isScrolled = false;

    onMount(() => {
        const element = document.getElementById("page_header") as HTMLElement;
        const height = element.offsetHeight;
        let previous_scroll_y = window.scrollY;

        window.addEventListener("scroll", () => {
            if (window.scrollY > previous_scroll_y) {
                isScrolled = true;
                element.style.transition = "top 0.5s";
                element.style.top = `-${height}px`;
            } else if (window.scrollY < previous_scroll_y) {
                isScrolled = false;
                element.style.transition = "top 0.5s";
                element.style.top = "0";
            }
            previous_scroll_y = window.scrollY;
        });
    });
</script>

<header id="page_header" class="page_header z-50">
    <nav class="main_nav">
        <menu>
            <a href="/" class="menu_item">
                <span class="active">Home</span>
            </a>
            <a href="#skills" class="menu_item">
                <span>Skills</span>
            </a>
            <!-- <a href="/portfolio" class="menu_item">
                <span>Portfolio</span>
            </a> -->
            <a href="#future_driven" class="menu_item">
                <span>Contact</span>
            </a>
        </menu>
    </nav>
</header>

<style lang="postcss">
    .page_header {
        position: fixed;
        left: 0;
        right: 0;
        top: 0;
        color: var(--dark);

        background-color: rgba(
            255,
            255,
            255,
            0.1
        ); /* Semi-transparent white color */
        backdrop-filter: blur(10px); /* Apply blur effect */

        @media screen and (max-width: 640px) {
            top: 100%;
        }

        .main_nav {
            display: flex;
            justify-content: center;

            menu {
                display: flex;
                gap: 1rem;
                padding: 1rem 0;

                span {
                    padding: 0.5rem 1rem;
                    &.active {
                        background-color: var(--grey-900);
                        color: var(--white);
                    }
                    &:hover:not(.active) {
                        background-color: var(--grey-600);
                        color: var(--white);
                    }
                    &:not(.active) {
                        color: var(--grey-200);
                    }
                }
            }
        }
    }
</style>
