<script>
  let todos = [
    { done: false, text: "finish svelte tutorial" },
    { done: false, text: "build app" },
    { done: false, text: "svelte mastery" }
  ];

  function add() {
    todos = todos.concat({ done: false, text: "" });
  }

  function clear() {
    todos = todos.filter(t => !t.done);
  }
  $: remaining = todos.filter(t => !t.done).length;
</script>

<style>
  .done {
    opacity: 0.4;
  }
</style>

<h1>todos</h1>

{#each todos as todo}
  <div class:done={todo.done}>
    <input type="checkbox" bind:checked={todo.done} />
    <input type="text" placeholder="what to do?" bind:value={todo.text} />
  </div>
{/each}

<button on:click={add}>add new</button>

<button on:click={clear}>clear completed</button>
