<script>
  const title = "Svelte";
  let suffix = $state("😀");

  const changeSuffix = () => {
    const emojis = ["😀", "🔥", "🌊", "🌲", "💰", "⛰️", "😎"];
    suffix = emojis.at(Math.floor(Math.random() * emojis.length));
  };
</script>

<h1>Hello, {title}! {suffix}</h1>
<button onclick={changeSuffix}>Change Emoji</button>
