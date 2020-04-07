<script>
  let m = { x: 0, y: 0 };

  function handleMousemove(event) {
    m.x = event.clientX;
    m.y = event.clientY;
  }
</script>

<style>
  div {
    width: 100%;
    height: 100%;
  }
</style>

move your mouse :)
<div on:mousemove={handleMousemove}>mouse position is {m.x} x {m.y}</div>
