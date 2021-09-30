<script>
    import data from '../data.json'
    import ItemComponent from '../components/ItemComponent.svelte';
</script>

{#each data as time}
    {#if time.timeframes.weekly}
        <ItemComponent 
            title={time.title} 
            current={time.timeframes.weekly.current}
            previous={time.timeframes.weekly.previous}
            color={time.color}
            image={time.image}
        />
    {/if}
{/each}