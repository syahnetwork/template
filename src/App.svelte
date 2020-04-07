<script>
  let count = 0;

  function countClick() {
    count += 1;
  }
</script>

<style>

</style>

<button on:click={countClick}>
  clicked {count} {count === 1 || count === 0 ? 'time' : 'times'}
</button>
