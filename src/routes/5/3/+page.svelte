<script>
  let brothers = [];
</script>

<ul>
  {#each brothers as bro, index (bro.id)}
    <li>{index}: {bro.name}（{bro.age}歳）</li>
  {:else}
    <li>兄弟はいません。</li>
  {/each}
</ul>
