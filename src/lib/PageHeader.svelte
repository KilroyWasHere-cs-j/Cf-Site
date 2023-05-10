<script lang="ts">
    export let header: string;
    export let subheader: string;
    export let subtext: string;
    import "../app.css"
</script>

<div class="flex flex-col w-screen mt-2 items-center justify-center px-6">
    <div class="flex flex-col items-center justify-center px-6">
        <h1 class="text-5xl font-bold text-center">{header}</h1>
        <div class="w-24 h-1 mt-4"></div>
        <p class="text-5sm font-bold text-center">{subheader}</p>
        <p class="text-3sm font-bold text-center">{subtext}</p>
        <div class="w-24 h-1 bg-blue-500 mt-4"></div>
        <p class="text-2sm font-bold text-center">B1</p>
    </div>
</div>