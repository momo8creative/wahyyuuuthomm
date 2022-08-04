<script>
  $: hidden = true;
  const handleClick = () => {
    hidden = false;
  };
</script>

<main class:show={hidden}>
  <button on:click={handleClick}>X</button>
  <h2 class="red">Warning !!!</h2>
  <p>Website dalam proses <span class="red">pengembangan.</span></p>
  <p>Mohon dimaklumi jika ada bug atau kekurangan.</p>

  <br />
  <a href="https://saweria.co/wathom"
    ><div>Buat beli jajan</div>
    <div class="link">https://saweria.co/wathom</div></a
  >
  <br />
  <p>
    Salam hangat <br />
    <small class="web">Web Developer : Momo Creative</small>
  </p>
</main>

<style>
  main.show {
    display: block !important;
  }

  main {
    display: none;
    position: fixed;
    z-index: 9;
    inset: 2rem;
    background-color: aliceblue;
    padding: 2rem;
    text-align: center;
  }

  main button {
    cursor: pointer;
    position: absolute;
    z-index: 99;
    top: 0;
    right: 0;
    width: 3rem;
    aspect-ratio: 1/1;
    font-weight: bold;
    font-size: 2rem;
  }

  @keyframes blink {
    100% {
      opacity: 0;
      transform: scale(120%);
    }
  }

  main h2 {
    color: red;
    padding: 2rem 0;
    animation: blink 1s linear infinite;
  }

  main p {
    padding: 1rem 0;
  }

  main .red {
    color: red;
  }

  main .web {
    font-size: 1.8rem;
  }

  main .link {
    text-decoration: underline;
    color: blue;
  }
</style>
