<script>
    import { fade, fly, scale, slide } from "svelte/transition";
    import Container from "./container.svelte";
    import { sineInOut } from "svelte/easing";
    let showMenu = false;
</script>

<div class="relative">
    <div class="bg-zinc-950 text-zinc-500 relative z-10">
        <div class="relative z-10">
            <Container>
                <nav
                    class="flex gap-4 items-center [&_a:hover]:text-zinc-50 [&_a]:transition-all"
                >
                    <a href="#/" class="text-lg">UMA Maths</a>
                    <ul class="hidden gap-4 sm:flex">
                        <li><a href="#/">About</a></li>
                        <li><a href="#/">Services</a></li>
                        <li><a href="#/">Contact</a></li>
                    </ul>
                    <button
                        on:click={() => (showMenu = !showMenu)}
                        class="ms-auto sm:hidden bg-zinc-800 rounded-lg transition-all hover:bg-zinc-700 p-1"
                        ><svg
                            xmlns="http://www.w3.org/2000/svg"
                            fill="none"
                            viewBox="0 0 24 24"
                            stroke-width="1.5"
                            stroke="currentColor"
                            class="w-6 h-6 text-white"
                        >
                            <path
                                stroke-linecap="round"
                                stroke-linejoin="round"
                                d="M3.75 6.75h16.5M3.75 12h16.5m-16.5 5.25h16.5"
                            />
                        </svg>
                    </button>
                </nav>
            </Container>
        </div>
    </div>
    {#if showMenu}
        <div
            transition:fly={{ y: "-100%", duration: 200, easing: sineInOut }}
            class="absolute w-full bottom-0 left-0 translate-y-full bg-zinc-950 text-zinc-500 border-t-2 border-zinc-800 sm:hidden z-0"
        >
            <Container>
                <ul
                    class=" gap-4 flex flex-col [&_a:hover]:text-zinc-50 [&_a]:transition-all"
                >
                    <li><a href="#/">About</a></li>
                    <li><a href="#/">Services</a></li>
                    <li><a href="#/">Contact</a></li>
                </ul>
            </Container>
        </div>
    {/if}
</div>
