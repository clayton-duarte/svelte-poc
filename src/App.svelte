<!-- JS -->
<script lang="ts">
  import Article from './components/Article.svelte'
  import Divider from './components/Divider.svelte'
  import Header from './components/Header.svelte'
  import Footer from './components/Footer.svelte'
  import Aside from './components/Aside.svelte'

  const year: number = new Date().getFullYear()
</script>

<!-- MARKUP -->
<main>
  <Header>WIP</Header>

  <div>
    <Aside />
    <Divider />
    <Article />
  </div>

  <Footer>WIP - {year}</Footer>
</main>

<!-- CSS -->
<style>
  main {
    grid-template-rows: auto 1fr auto;
    display: grid;
    height: 100%;
    gap: 1rem;
  }

  div {
    grid-template-columns: auto auto 1fr;
    max-width: 1280px;
    padding: 0 1rem;
    margin: 0 auto;
    display: grid;
    width: 100%;
    gap: 1rem;
  }
</style>
