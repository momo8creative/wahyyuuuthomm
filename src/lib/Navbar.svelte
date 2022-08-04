<script>
  import imgUrl from "$lib/assets/foto_profil_wahyu.png";
</script>

<header>
  <img src={imgUrl} alt="profil" />
  <div class="title">Welcome to my website</div>
  <small class="subtitle">Let's join us</small>
</header>

<style>
  header {
    text-align: center;
    border-bottom: 3px solid black;
    text-transform: uppercase;
  }

  header img {
    width: 9rem;
    padding: 1rem 0;
  }

  header .title {
    font-size: 2.2rem;
    line-height: 0;
  }

  header .subtitle {
    font-size: 1.6rem;
  }
</style>
