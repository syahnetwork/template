<script>
  let count = 0;

  $: if (count >= 10) {
    alert("count >=10 , back to 9");
    count = 9;
  }

  function clickHandler() {
    count += 1;
  }
</script>

<style>

</style>

<button on:click={clickHandler}>
  clicked {count} {count === 1 || count === 0?'time':'times'}
</button>
