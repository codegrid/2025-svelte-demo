<script>
  let message = $state(null);
  function handleKeyDown(event) {
    if (event.key === "Enter") {
      message = "Enterキーが押されました";
    } else if (event.key === "Escape") {
      message = "Escapeキーが押されました";
    } else {
      message = null;
    }
  }
</script>

<label>
  何か入力してください:
  <input onkeydown={handleKeyDown} />
</label>

{#if message !== null}
  <p>{message}</p>
{/if}
