<script>
  let count = $state(0);

  function onClickButton() {
    count++;
  }
</script>

<button type="button" onclick={onClickButton}>Count up</button>

{count}
