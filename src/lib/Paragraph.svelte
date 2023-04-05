<script lang="ts">
    export let header: string = "";
    export let text: string = "";
    import "../app.css";
</script>

<div class="flex flex-col w-screen mt-2 items-center justify-center px-6">
    <h1 class="text-5xl font-bold text-center mt-5">{header}</h1>
    <p class="text-5sl font-bold text-center">{text}</p>
</div>
