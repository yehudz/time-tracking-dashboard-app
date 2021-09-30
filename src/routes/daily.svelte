<script>
    import data from '../data.json'
    import ItemComponent from '../components/ItemComponent.svelte';
</script>
{#each data as time}
    {#if time.timeframes.daily}
        <ItemComponent 
            title={time.title} 
            current={time.timeframes.daily.current}
            previous={time.timeframes.daily.previous}
            color={time.color}
            image={time.image}
        />
    {/if}
{/each}
