<script>
  let count = $state(0);

  function onClickButton() {
    count += 1;
  }
</script>

<div>
  <output>{count}</output>
</div>
<button onclick={onClickButton}>button</button>

<style>
  /* 必要なければstyleタグごと消してよい */
</style>
