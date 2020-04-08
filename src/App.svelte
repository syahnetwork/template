<script>
  import Outer from "./Outer.svelte";

  function handleMessage(event) {
    alert(event.detail.text);
  }
</script>

<Outer on:message={handleMessage} />
<!-- call object hello from outer which has inner components -->