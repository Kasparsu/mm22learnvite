<script>
    import ItemList from "./ItemList.svelte";
    let message = '';
    let items = [
        { name: 'leib', isDone: true },
        { name: 'sai', isDone: false },
        { name: 'piim', isDone: false },
        { name: 'viin', isDone: true },
    ];
    $: doneItems = items.filter(item => item.isDone);
    $: todoItems = items.filter(item => !item.isDone);
    function addItem(){
        items.push(message);
        items=items;
        message='';
    }

</script>

<div class="container">
    <div class="input-group mt-3">
        <input type="text" class="form-control" bind:value={message}>
        <button class="btn btn-primary" on:click={addItem}>Click me!</button>
    </div>
    <ItemList title="All Items" bind:items={items} />
    <ItemList title="Done Items" bind:items={doneItems}/>
    <ItemList title="Todo Items" bind:items={todoItems}/>
</div>
<style>

</style>