<script>
  function handleClick(event) {
    const target = event.target;
    if (target.classList.contains("active")) {
      target.classList.remove("active");
    } else {
      target.classList.add("active");
    }
  }
</script>

<button type="button" onclick={handleClick}
  >クリックするとテキストの色が変わります</button
>

<style>
  :global .active {
    color: red;
  }
</style>
