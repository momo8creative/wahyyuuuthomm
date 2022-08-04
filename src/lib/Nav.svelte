<script>
  const menus = [
    {
      label: "Photography",
      to: "https://drive.google.com/drive/folders/14b9hsYtcwre9I9OhnqV4RbgdSy1RO9CO?usp=sharing",
      icon: "camera",
    },
    {
      label: "Videography",
      to: "https://drive.google.com/drive/folders/1U36B-2Fc75laszdLA_Hf_Gb_7WdGJ06x?usp=sharing",
      icon: "camera",
    },
    {
      label: "Design Grafis",
      to: "https://drive.google.com/drive/folders/1yRh_CyYsqdIiTnjv7tV6TIw3ioLglGMc?usp=sharing",
      icon: "camera",
    },
    { label: "About Me", to: "/aboutme", icon: "camera" },
  ];
</script>

<nav>
  {#each menus as menu}
    <a href={menu.to}> <div>{menu.label}</div></a>
  {/each}
</nav>

<style>
  nav {
    text-transform: uppercase;
    display: flex;
    flex-direction: column;
    gap: 1.4rem;
  }

  nav a > div {
    display: flex;
    justify-content: center;
    align-items: center;
    font-size: 3rem;
    height: 6rem;
    border: 2px solid black;
    border-radius: 1rem;
    box-shadow: 0 0 2px black;
  }
</style>
