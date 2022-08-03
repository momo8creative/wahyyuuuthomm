<script>
  import Icon from "$lib/Icon.svelte";

  const menus = [
    { label: "Photography", to: "/", icon: "camera" },
    { label: "Videography", to: "/", icon: "camera" },
    { label: "Design", to: "/", icon: "camera" },
    { label: "Youtube", to: "/", icon: "camera" },
    { label: "About Me", to: "/", icon: "camera" },
  ];
</script>

<main>
  <header>
    <h1>WahyyuuuThomm</h1>
    <p>My Portofolio Website</p>
  </header>

  <nav>
    {#each menus as menu}
      <a href="/" class="link"> <div>{menu.label}</div></a>
    {/each}
  </nav>

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
    height: 100vh;

    margin: 0 auto;
  }

  header {
    padding: 4rem 0;
    text-align: center;
  }

  nav {
    display: flex;
    flex-direction: column;
    gap: 2rem;
    width: max-content;
  }

  a.link {
    font-size: 2.8rem;
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 1rem;
    position: relative;
    text-decoration: none;
    background-color: #cccccc;
    color: black;
    height: 5rem;
    width: 20rem;
    text-transform: uppercase;
  }

  a.link::before {
    content: "";
    position: absolute;
    z-index: -1;
    width: 100%;
    height: 100%;
    right: -0.8rem;
    bottom: -0.8rem;
    background-color: hsl(0, 0%, 40%);
  }

  footer {
    font-family: "Cute Font", cursive;
    margin-top: auto;
    padding: 2rem 0;
    text-align: center;
    line-height: 1.8rem;
  }
</style>
