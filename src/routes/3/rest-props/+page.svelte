<script>
  import LabeledButton from "./LabeledButton.svelte";
</script>

<p>
  ボタンをクリックするとコンソールにログが出力されます。<br />
  コンソールを開いて確認してください。
</p>

<LabeledButton
  label="Click Me"
  type="button"
  onclick={() => console.log("Button clicked!")}
  class="btn"
/>
