<script lang="ts">
    import Container from "./container.svelte";
</script>

<div class="grid place-content-center py-8 border-y border-zinc-300">
    <div>
        <ul class="flex divide-x-2 border">
            <li>
                <a href="#/"
                    ><svg
                        xmlns="http://www.w3.org/2000/svg"
                        fill="none"
                        viewBox="0 0 24 24"
                        stroke-width="1.5"
                        stroke="currentColor"
                        class="size-4"
                    >
                        <path
                            stroke-linecap="round"
                            stroke-linejoin="round"
                            d="m18.75 4.5-7.5 7.5 7.5 7.5m-6-15L5.25 12l7.5 7.5"
                        />
                    </svg>
                </a>
            </li>
            <li class="!bg-sky-400 text-white"><a href="#/">1</a></li>
            <li><a href="#/">2</a></li>
            <li><a href="#/">3</a></li>
            <li><a href="#/">4</a></li>
            <li><a href="#/">5</a></li>
            <li>
                <a href="#/"
                    ><svg
                        xmlns="http://www.w3.org/2000/svg"
                        fill="none"
                        viewBox="0 0 24 24"
                        stroke-width="1.5"
                        stroke="currentColor"
                        class="size-4"
                    >
                        <path
                            stroke-linecap="round"
                            stroke-linejoin="round"
                            d="m5.25 4.5 7.5 7.5-7.5 7.5m6-15 7.5 7.5-7.5 7.5"
                        />
                    </svg>
                </a>
            </li>
        </ul>
    </div>
</div>
<Container>
    <p class="my-12 text-zinc-800 text-sm">Copyright &copy; UMA Maths 2024</p>
</Container>

<style lang="postcss">
    li {
        @apply size-8  grid place-content-center transition-all hover:bg-zinc-200;
    }
</style>
