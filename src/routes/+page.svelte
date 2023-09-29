<script>
    let count = 0;
</script>

<h1>Main page</h1>
<button><a href="./about">About</a></button>

<div>
    <p>Counter : {count}</p>
    <button on:click={()=> count+=1}>Increase</button>
    <button on:click={()=> count-=1}>Decrease</button>
</div>

<style>
    h1{
        text-align: center;
    }
</style>