<script>
  import ExampleComponent from "./ExampleComponent.svelte";
</script>

<div class="App">
  <h1 class="title">Svelte</h1>
  <p class="description">web development for the rest of us</p>
  <ExampleComponent />
</div>

<style>
  :global(body) {
    color: salmon;
  }

  .App {
    text-align: center;
  }

  .title {
    margin-bottom: 0;
    color: tomato;
    font-size: 3rem;
    line-height: 1;
  }

  .description {
    font-size: 1.2rem;
  }
</style>
