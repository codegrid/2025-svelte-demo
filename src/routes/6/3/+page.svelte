<script>
  let brothers = [
    {
      id: "ichiro",
      name: "一郎",
      age: 20,
    },
    {
      id: "jiro",
      name: "二郎",
      age: 18,
    },
    {
      id: "saburo",
      name: "三郎",
      age: 12,
    },
  ];
</script>

<ul>
  {#each brothers as bro, index (bro.id)}
    <li>{index + 1}: {bro.name}（{bro.age}歳）</li>
  {:else}
    <li>兄弟はいません。</li>
  {/each}
</ul>
