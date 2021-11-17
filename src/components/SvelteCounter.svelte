<script>
  let count = 0;

  function add() {
    count += 1;
  }

  function subtract() {
    count -= 1;
  }
</script>

<div id="svelte" class="counter">
  <button on:click={subtract}>–</button>
  <pre>{ count }</pre>
  <button on:click={add}>+</button>
</div>

<style>
  button {
    transform: scale(1.5);
    border: 12px double black;
    cursor:pointer;
  }
</style>