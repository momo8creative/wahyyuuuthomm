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
    {
      label: "Youtube",
      to: "https://www.youtube.com/c/NDRENGUSMUSICOFFICIAL",
      icon: "camera",
    },
    { label: "About Me", to: "/aboutme", icon: "camera" },
  ];
</script>

<nav>
  {#each menus as menu}
    <a href={menu.to} class="link"> <div>{menu.label}</div></a>
  {/each}
</nav>

<style>
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
</style>
