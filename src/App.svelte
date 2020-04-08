<script>
function handleClick() {
  alert('no more alerts')
}
</script>
<!-- give rule only once -->
<button on:click|once={handleClick}>
click me

</button>