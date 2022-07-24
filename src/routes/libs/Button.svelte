<script>
  export let onClick = () => {};
  export let spanRow = false;
  export let type = "number";
</script>

<style>
  .spanRow {
    grid-column: 1 / -1;
  }

  .number {
    background-color: rgb(8, 72, 246);
  }

  .operator {
    background-color: #ff4561;;
  }

  .action {
    background-color: gray;
  }

  h2 {
    color: #fff;
  }
</style>

<button class={type} class:spanRow on:click={onClick}>
  <h2>
    <slot>¯\_(ツ)_/¯</slot>
  </h2>
</button>