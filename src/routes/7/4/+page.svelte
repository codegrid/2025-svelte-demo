<script>
  let result = $state(null);

  function handleSubmit(event) {
    event.preventDefault();

    result = {
      name: event.target.name.value,
      favorite: event.target.favorite.value,
    };
  }
</script>

<form onsubmit={handleSubmit}>
  <label>
    名前:
    <input type="text" name="name" />
  </label>
  <label>
    好きなもの:
    <input type="text" name="favorite" />
  </label>

  <button>送信</button>
</form>

{#if result !== null}
  <div>入力内容: {JSON.stringify(result)}</div>
{/if}
