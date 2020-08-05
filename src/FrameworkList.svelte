<script>
  let frameworks = [
    { id: 1, name: 'Svelte' },
    { id: 2, name: 'Angular' },
    { id: 3, name: 'React' },
    { id: 4, name: 'Vue' },
  ];
</script>

<style>
  .list {
    width: 300px;
    margin: 0 auto;
    text-align: left;
  }
</style>

<h1>List of Frameworks</h1>
<div class="list">
  <ul>
    {#each frameworks as { id, name }}
      <li>{id}: {name}</li>
    {/each}
  </ul>
</div>
