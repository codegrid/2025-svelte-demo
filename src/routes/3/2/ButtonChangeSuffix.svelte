<script>
  let { suffix = $bindable() } = $props();

  const changeSuffix = () => {
    const emojis = ["😀", "🔥", "🌊", "🌲", "💰", "⛰️", "😎"];
    suffix = emojis.at(Math.floor(Math.random() * emojis.length));
  };
</script>

<button onclick={changeSuffix}>Change Emoji</button>
