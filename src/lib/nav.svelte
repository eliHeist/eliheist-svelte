<header class="page_header z-50">
    <nav class="main_nav">
        <menu>
            <a href="/" class="menu_item">
                <span class="active">Home</span>
            </a>
            <a href="/about" class="menu_item">
                <span>About</span>
            </a>
            <a href="/portfolio" class="menu_item">
                <span>Portfolio</span>
            </a>
            <a href="/contact" class="menu_item">
                <span>Contact</span>
            </a>
        </menu>
    </nav>
</header>

<button
    title="Menu button"
    class="hamburger-btn grid grid-flow-col sm:hidden z-50"
    aria-expanded="false">
    <!-- <svg class="hamburger w-10" fill="none" viewbox="-10 -10 120 120">
        <path class="line" d="m 20 40 h 60 a 1 1 0 0 1 0 20 h -60 a 1 1 0 0 1 0 -40 h 30 v 70"></path>
    </svg> -->
    <div class="text-primary-500 h-full grid content-center pr-2 text-sm">
        <span>Menu</span>
    </div>
</button>

<style lang="postcss">
    .page_header {
        position: fixed;
        left: 0;
        right: 0;
        top: 0;
        color: var(--dark);
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
                }
            }
        }
    }
</style>
