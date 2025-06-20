<script>
  import Header from "./Header.svelte";

  const title = "Svelte";
  let suffix = $state("😀");

  const changeSuffix = () => {
    const emojis = ["😀", "🔥", "🌊", "🌲", "💰", "⛰️", "😎"];
    suffix = emojis.at(Math.floor(Math.random() * emojis.length));
  };
</script>

<Header {title} {suffix} />
<button onclick={changeSuffix}>Change Emoji</button>
