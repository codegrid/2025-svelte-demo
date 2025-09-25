<script>
  import { onMount } from "svelte";
  let dynamicDiv;

  // コンポーネントが読み込まれたときに、divのクラスを操作している
  onMount(() => dynamicDiv.classList.add("used"));
</script>

<div class="App">
  <!-- DOMを直接操作できるように`dynamicDiv`変数へ格納している -->
  <div bind:this={dynamicDiv}>Dynamic</div>
</div>

<style>
  .App {
    font-size: 24px;
  }

  .used {
    color: blue;
  }
</style>
