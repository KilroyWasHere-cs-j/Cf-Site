<script lang="ts">
    export let height: string;
    import "../app.css";
</script>

<div class="w-screen h-{height}">
    <slot/>
</div>
