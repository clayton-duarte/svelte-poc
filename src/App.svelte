<!-- JS -->
<script lang="ts">
  import Header from './components/Header.svelte'
  import Footer from './components/Footer.svelte'

  let name: string = 'clayton'
  let times: number = 0

  function onClick() {
    times++
  }
</script>

<!-- MARKUP -->
<Header />

<main>
  <h1>Hello {name}!</h1>
  <button on:click={onClick}>clicked {times}</button>
</main>

<Footer />

<!-- CSS -->
<style>
  main {
    text-align: center;
    margin: 0 auto;
    padding: 1em;
  }

  h1 {
    text-transform: uppercase;
    font-weight: 100;
    color: tomato;
    font-size: 4em;
  }
</style>
