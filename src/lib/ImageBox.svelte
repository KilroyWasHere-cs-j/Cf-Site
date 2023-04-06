<script lang="ts">
    export let src: string;
    export let width: string = "80";
    export let height: string = "80";
    import "../app.css"
</script>

<div class="flex flex-row">
    <div class="h-{height} w-{width} p-2">
        <img src="{src}" alt="Someone stole my image"/>
    </div>
    <div>
        <slot/>
    </div>
</div>