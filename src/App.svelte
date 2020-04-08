<script>
  let name = "";
</script>

<input type=" text" bind:value={name} placeholder="enter name" />
<p>hello {name || 'stranger'}!</p>
