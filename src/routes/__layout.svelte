<script>
  import "../styles/global.css";
</script>

<svelte:head>
  <title>WahyyuuuThomm</title>
</svelte:head>

<main>
  <header>
    <a href="/">
      <h1>WahyyuuuThomm</h1>
    </a>
    <p>My Portofolio Website</p>
  </header>

  <slot />

  <footer>
    <h3>Design By</h3>
    <div>Web Developer : Momo Creative</div>
    <div>Design Grafis : Wahyyuuuthomm</div>
  </footer>
</main>

<style>
  main {
    display: flex;
    flex-direction: column;
    align-items: center;
    margin: 0 auto;
  }

  header {
    padding: 4rem 0;
    text-align: center;
  }

  header a h1 {
    transition: all 300ms ease;
  }

  header a h1:hover {
    transform: scale(105%);
  }

  footer {
    font-family: "Cute Font", cursive;
    margin-top: auto;
    padding: 6rem 0 8rem 0;
    text-align: center;
    line-height: 1.8rem;
  }
</style>
