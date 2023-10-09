<script>
    let count = 0;
    function click(){
        count++;
    }
</script>

<button class="btn btn-primary" on:click={click}>Click me!</button>
<h1>{ count }</h1>

<style>

</style>