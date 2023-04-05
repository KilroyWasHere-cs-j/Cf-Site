<script lang="ts">
    export let width: string;
    export let height: string;
    export let char: string = "";
    export let imagePath: string = "";
    import "../app.css";
</script>

<div class="flex flex-col w-screen my-48 items-center justify-center px-6 w={width} h={height} bg-cover" style="background-image: url({imagePath}); height: {height}">
    <h1 class="text-4xl font-bold text-center">{char}</h1>
</div>