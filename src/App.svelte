<script>
  let count = 1;

  //the $: means re run whenever these values change
  $: doubled = count * 2;
  $: quadrupled = doubled * 2;
  $: sixTimes = quadrupled * 2;
  function clickHandler() {
    count += 1;
  }
</script>

<style>

</style>

<button on:click={clickHandler}>count:{count}</button>

<p>{count}*2={doubled}</p>
<p>{doubled}*2={quadrupled}</p>
<p>{quadrupled}*2={sixTimes}</p>
