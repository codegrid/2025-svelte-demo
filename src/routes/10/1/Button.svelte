<script>
  let { priority } = $props();
</script>

<button class={priority}>Click</button>

<style>
  .primary {
    color: tomato;
  }
  .secondary {
    color: lime;
  }
  .tertiary {
    color: cornflowerblue;
  }
</style>
