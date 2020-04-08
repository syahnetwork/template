<script>
  let yes = false;
</script>

<label for="">
  <input type="checkbox" bind:checked={yes} />
  yes , send email
</label>

{#if yes}
  <p>thanks, will send email</p>
{:else}
  <p>we won't send email</p>
{/if}

<button disabled={!yes}>subscribe</button>
