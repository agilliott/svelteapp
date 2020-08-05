<script>
  let m = { x: 0, y: 0 };
  function handleMousemove(event) {
    m.x = event.clientX;
    m.y = event.clientY;
  }
</script>

<style>
  div {
    width: 300px;
    height: 300px;
    margin: 0 auto;
    color: #ff3e00;
    border: 1px solid #ff3e00;
  }
</style>

<h1>Mouse hunter</h1>
<div on:mousemove={handleMousemove}>The mouse position is {m.x} x {m.y}</div>
