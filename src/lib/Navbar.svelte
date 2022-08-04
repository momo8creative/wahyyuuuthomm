<script>
  import imgUrl from "$lib/assets/foto_profil_wahyu.png";
</script>

<header>
  <img src={imgUrl} alt="profil" />
  <br />
  <div class="text">
    <span class="title">Welcome to my website</span>
    <span class="subtitle">Let's join us</span>
  </div>
</header>

<style>
  header {
    text-align: center;
    border-bottom: 3px solid black;
    text-transform: uppercase;
  }

  header .text {
    display: flex;
    flex-direction: column;
  }

  header img {
    width: 9rem;
    padding: 1rem 0;
  }

  header .title {
    font-size: 2.2rem;
    line-height: 1.8rem;
  }

  header .subtitle {
    font-size: 1.6rem;
  }
</style>
