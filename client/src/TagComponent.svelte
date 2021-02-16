<script>
    export let tags = [];
    import Tag from './Tag.svelte';
    import TagView from './TagView.svelte';
</script>

<div class="tag-container flex items-start content-start flex-wrap overflow-auto">
    <TagView/>
    {#each tags as tag}
        <Tag {...tag}/>
    {/each}
</div>

<style>
    .tag-container {
        height: 100%;
    }
</style>
