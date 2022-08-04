<script>
  import Icon from "$lib//Icon.svelte";

  //   let icons = ["tiktok", "youtube", "instagram", "twitter"];
  let icons = [
    { name: "tiktok", width: 30 },
    { name: "youtube", width: 36 },
    { name: "instagram", width: 36 },
    { name: "twitter", width: 36 },
  ];
</script>

<section class="icon-group">
  {#each icons as icon}
    <div class={`icon ${icon.name}`}>
      <Icon name={icon.name} with={icon.width} height={icon.width} />
    </div>
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
