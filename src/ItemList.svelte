<script>

    export let title;
    export let items;

</script>

<h1>{title}</h1>
<ul>
    {#each items as item}
        <li>{item.name} <input type="checkbox" class="form-check-input" bind:checked={item.isDone} ></li>
    {/each}
</ul>