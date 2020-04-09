<script>
  let questions = [
    { id: 1, text: `where go to school?` },
    { id: 2, text: `what is your mother's name?` },
    { id: 3, text: `what is googling?` }
  ];

  let selected;
  let answer = "";

  function handleSubmit() {
    alert(
      `answered question ${selected.id} (${selected.text}) with "${answer}"`
    );
  }
</script>

<style>
  input {
    display: block;
    width: 500px;
    max-width: 100%;
  }
</style>

<h2>insecurity questions</h2>

<form action="" on:submit|preventDefault={handleSubmit}>
  <select name="" id="" bind:value={selected} on:change={() => (answer = '')}>

    {#each questions as question}
      <option value={question}>{question.text}</option>
    {/each}

  </select>

  <input type="text" bind:value={answer} />

  <button disabled={!answer} type="submit">submit</button>

  <p>selected question {selected ? selected.id : '[waiting...]'}</p>

</form>
