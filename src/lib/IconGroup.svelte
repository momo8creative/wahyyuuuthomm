<script>
  import Icon from "$lib//Icon.svelte";

  //   let icons = ["tiktok", "youtube", "instagram", "twitter"];
  let icons = [
    {
      name: "tiktok",
      to: "https://www.tiktok.com/@ndrengusmusicteam?_t=8UXz0s21s9a&_r=1",
      title: "Tiktok : @ndrengusmusicteam",
      width: 30,
    },
    {
      name: "youtube",
      to: "https://www.youtube.com/c/NDRENGUSMUSICOFFICIAL",
      title: "Youtube : NDRENGUSMUSICOFFICIAL",
      width: 36,
    },
    {
      name: "instagram",
      to: "https://instagram.com/wahyyuuuthomm?igshid=YmMyMTA2M2Y=",
      title: "IG : wahyyuuuthomm",
      width: 36,
    },
    {
      name: "twitter",
      to: "https://twitter.com/WahyuTomm?t=TjjAbg-LPMuzkjixPL6lnQ&s=09",
      title: "Twitter : WahyuTomm",
      width: 36,
    },
  ];
</script>

<section class="icon-group">
  {#each icons as icon}
    <a href={icon.to} class={`icon ${icon.name}`} title={icon.title}>
      <Icon name={icon.name} with={icon.width} height={icon.width} />
    </a>
  {/each}
</section>

<style>
  .icon-group {
    display: flex;
    justify-content: space-between;
    padding: 2rem 0;
  }

  .icon {
    /* background-color: gray; */
    /* border: 1px solid red; */
    display: flex;
    justify-content: center;
    align-items: center;
  }
</style>
