<script>
    import Container from "./container.svelte";
</script>

<Container>
    <p class="flex gap-2 items-end border-b border-zinc-300 mb-4 pb-2">
        <span class="text-4xl font-bold text-zinc-900">3 Col Portfolio</span>
        <span class="text-2xl text-zinc-500">Showcase Your Work</span>
    </p>
    <div class="grid lg:grid-cols-3 gap-4">
        <div class="space-y-4">
            <div
                class="aspect-[7/4] bg-zinc-500 grid place-content-center text-zinc-600 text-3xl font-bold"
            >
                700 x 400
            </div>
            <div>
                <p class="text-sky-500 text-3xl font-bold">Project Name</p>
                <p class="text-sm mt-4">
                    Lorem ipsum dolor sit amet consectetur adipisicing elit.
                    Quidem
                </p>
            </div>
        </div>
        <div class="space-y-4">
            <div
                class="aspect-[7/4] bg-zinc-500 grid place-content-center text-zinc-600 text-3xl font-bold"
            >
                700 x 400
            </div>
            <div>
                <p class="text-sky-500 text-3xl font-bold">Project Name</p>
                <p class="text-sm mt-4">
                    Lorem ipsum dolor sit amet consectetur adipisicing elit.
                    Quidem
                </p>
            </div>
        </div>
        <div class="space-y-4">
            <div
                class="aspect-[7/4] bg-zinc-500 grid place-content-center text-zinc-600 text-3xl font-bold"
            >
                700 x 400
            </div>
            <div>
                <p class="text-sky-500 text-3xl font-bold">Project Name</p>
                <p class="text-sm mt-4">
                    Lorem ipsum dolor sit amet consectetur adipisicing elit.
                    Quidem
                </p>
            </div>
        </div>
    </div>
</Container>
