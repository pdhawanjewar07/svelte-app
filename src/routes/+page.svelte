<script>
    let count=0;
</script>

<h1>Counter : {count}</h1>
<button on:click={()=> count+=1}>Increase</button>
<button on:click={()=> count-=1}>Decrease</button>