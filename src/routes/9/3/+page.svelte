<div class="App">
  <div class={Date.now() % 2 === 0 ? "even" : "odd"}>Even or Odd</div>
</div>

<style>
  .App {
    font-size: 24px;
  }

  .even {
    color: green;
  }

  .odd {
    color: red;
  }
</style>
