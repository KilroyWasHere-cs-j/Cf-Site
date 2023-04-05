<script lang="ts">
    export let header: string;
    import "../app.css"
	import Bar from "./Bar.svelte";
</script>

<div class="flex flex-col w-screen mt-2 items-center justify-center px-6">
    <div class="flex flex-col items-center justify-center px-6">
        <h1 class="text-5xl font-bold text-center">{header}</h1>
        <Bar color=gray/>
    </div>
</div>