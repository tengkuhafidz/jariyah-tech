<script>
    import Card from "./Card.svelte";
    import {projects} from "./data";
</script>

<div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-y-4 md:gap-x-8 lg:gap-x-16 py-24">
    {#each projects as project (projects)}
        <Card {...project}/>
    {/each}
</div>
