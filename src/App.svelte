<script>
  import Keypad from "./Keypad.svelte";

  let pin;
  $: view = pin ? pin.replace(/\d(?!$)/g, "•") : "enter your pin";

  function handleSubmit() {
    alert(`submitted ${pin}`);
  }
</script>

<h1 style="color:{pin ? 'orange' : 'red'}">{view}</h1>

<Keypad bind:value={pin} on:submit={handleSubmit} />
