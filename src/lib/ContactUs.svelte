<script>
  import Icon from "$lib/Icon.svelte";
</script>

<section>
  <div class="title">Contact us</div>
  <article>
    <div class="icon">
      <Icon name="mail" width="22" />
    </div>
    <div class="link">{@html "wahyuthomasadiprastyo@gmail.com"}</div>
  </article>
  <article>
    <div class="icon">
      <Icon name="whatsapp" width="22" />
    </div>
    <div class="link">wa.me/6282211258533</div>
  </article>
</section>

<style>
  section {
    width: 36rem;
    margin: 0 auto;
    padding: 2rem;
    font-size: 1.8rem;
  }

  section .title {
    padding: 1rem 0;
  }

  section article {
    display: flex;
    gap: 1rem;
    align-items: center;
    height: 3rem;
    padding: 0 1rem;
  }

  section .link {
    color: blue;
    text-decoration: underline;
  }
</style>
