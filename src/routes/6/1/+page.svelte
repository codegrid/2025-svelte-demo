<script>
  let payment = $state("card");

  const onChangeSelect = (event) => {
    payment = event.target.value;
  };
</script>

<form>
  <select onchange={onChangeSelect}>
    <option value="card">クレジットカード</option>
    <option value="digital_currency">電子マネー</option>
    <option value="others">その他</option>
  </select>
</form>

<div>
  {#if payment === "card"}
    <p>クレジットカードの設定にお進みください。</p>
  {:else if payment === "digital_currency"}
    <p>電子マネーを選択してください。</p>
  {:else}
    <p>お問い合わせください。</p>
  {/if}
</div>
