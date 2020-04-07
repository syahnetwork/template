<script>
  let user = { loggedIn: false };

  function toggle() {
    user.loggedIn = !user.loggedIn;
    console.log("ADAM LOGIN === " + user.loggedIn);
  }
</script>

{#if user.loggedIn}
  <button on:click={toggle}>log out</button>
<!-- {/if} -->
{:else}
<!-- {#if !user.loggedIn} -->
  <button on:click={toggle}>log in</button>
{/if}
