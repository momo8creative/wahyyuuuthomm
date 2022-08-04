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
  <a href="/" class="saweria"><span>LINK SAWERIA</span></a>
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
    position: absolute;
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

  main .saweria {
    font-family: Impact, Haettenschweiler, "Arial Narrow Bold", sans-serif;
    font-size: 3.4rem;
    color: white;
    text-shadow: 0 0 4px black, 0 0 2px black, 0 0 2px black, 0 0 4px black,
      0 0 2px black;
    display: flex;
    justify-content: center;
    align-items: center;
  }

  main .saweria span {
    position: absolute;
    width: max-content;
    transform: rotate(-2deg);
  }
</style>
