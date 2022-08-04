<script>
  import "../styles/global.css";
  import Navbar from "$lib/Navbar.svelte";
  import IconGroup from "$lib/IconGroup.svelte";
  // import Nav from "$lib/Nav.svelte";
  import FooterBot from "$lib/FooterBot.svelte";
  import Popup from "$lib/Popup.svelte";
  import ContactUs from "$lib/ContactUs.svelte";
</script>

<svelte:head>
  <title>WahyyuuuThomm</title>
</svelte:head>

<!-- <Popup /> -->
<main>
  <Navbar />
  <IconGroup />
  <slot />
  <!-- <Nav /> -->
</main>

<ContactUs />

<FooterBot />

<style>
  main {
    width: 26rem;
    margin: 0 auto;
  }
</style>
