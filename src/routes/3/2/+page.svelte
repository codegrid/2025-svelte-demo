<script>
  import Header from "./Header.svelte";
  import ButtonChangeSuffix from "./ButtonChangeSuffix.svelte";

  const title = "Svelte";
  let suffix = $state("😀");
</script>

<Header {title} {suffix} />
<ButtonChangeSuffix bind:suffix />
