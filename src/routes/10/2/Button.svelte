<script>
  let { disabled } = $props();
</script>

<button class={disabled ? "disabled" : "enabled"}> Click </button>

<style>
  .enabled {
    background-color: #f0f0f0;
  }
  .disabled {
    background-color: #9e9e9e;
  }
</style>
