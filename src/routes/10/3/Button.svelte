<script>
  let { priority, size, disabled } = $props();
</script>

<button class="btn {priority} {size}" class:enabled={!disabled} class:disabled
  >Click</button
>

<style>
  .btn {
    cursor: pointer;
  }

  .primary {
    color: tomato;
  }
  .secondary {
    color: lime;
  }
  .tertiary {
    color: cornflowerblue;
  }

  .large {
    font-size: 24px;
  }
  .medium {
    font-size: 16px;
  }
  .small {
    font-size: 14px;
  }

  .enabled {
    background-color: #f0f0f0;
  }
  .disabled {
    background-color: #9e9e9e;
  }
</style>
