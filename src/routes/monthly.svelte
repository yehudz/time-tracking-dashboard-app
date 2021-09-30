<script>
    import data from '../data.json'
    import ItemComponent from '../components/ItemComponent.svelte';
</script>

{#each data as time}
    {#if time.timeframes.monthly}
        <ItemComponent 
            title={time.title} 
            current={time.timeframes.monthly.current}
            previous={time.timeframes.monthly.previous}
            color={time.color}
            image={time.image}
        />
    {/if}
{/each}