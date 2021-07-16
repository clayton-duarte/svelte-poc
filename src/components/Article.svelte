<!-- JS -->
<script lang="ts">
  let stats = {
    for: 1,
    hab: 1,
    res: 1,
    arm: 1,
    pdf: 1,
  }
</script>

<!-- MARKUP -->
<article>
  <h1>Stats</h1>
  <ul>
    {#each Object.entries(stats) as [key, value]}
      <li>
        <strong>{key}</strong>
        <span>{value}</span>
      </li>
    {/each}
  </ul>
</article>

<!-- CSS -->
<style>
  article {
    align-content: start;
    display: grid;
    gap: 1rem;
  }

  ul {
    padding: 0 0 0 1rem;
    list-style: none;
    margin: 0;
    display: grid;
    gap: 1rem;
  }

  li {
    grid-template-columns: 1fr 1fr;
    display: grid;
    gap: 1rem;
  }

  strong {
    text-transform: uppercase;
  }
</style>
