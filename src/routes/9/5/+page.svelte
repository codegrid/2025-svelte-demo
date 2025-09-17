<script>
  import { onMount } from "svelte";
  let dynamicDiv;

  // コンポーネントが読み込まれたときに、divのクラスを操作している
  onMount(() => dynamicDiv.classList.add("used"));
</script>

<!-- DOMを直接操作できるように`dynamicDiv`変数へ格納している -->
<div bind:this={dynamicDiv}>Dynamic</div>

<style>
  .used {
    color: blue;
  }
</style>
