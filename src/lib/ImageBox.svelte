<script lang="ts">
    export let src: string;
    export let width: string;
    export let height: string;
    import "../app.css"
</script>

<div class="flex flex-row scale-75">
    <div class="h-{height} w-{width} p-2">
        <!-- svelte-ignore a11y-img-redundant-alt -->
        <img class= "scale-100 object-fit" src="{src}" alt="Someone stole my image"/>
    </div>
    <div>
        <slot/>
    </div>
</div>