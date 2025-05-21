<script>
  const makeHeader = (title, suffix) => {
    return `Hello, ${title}! ${suffix}`;
  };
</script>

<h1>{makeHeader("Svelte", "😀")}</h1>
