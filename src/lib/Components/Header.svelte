<script>
  import svelte from "../../assets/svelte.svg";
  let Data = [
    {
      id: 1,
      link: "Home",
    },
    {
      id: 2,
      link: "Pricing",
    },
    {
      id: 3,
      link: "Testimony",
    },
  ];
</script>

<header class="header">
  <img src={svelte} class="header_image" alt="" />
  <div class="navigation">
    {#each Data as data (data.id)}
      <a href="/" class="nav-links">{data.link}</a>
    {/each}
  </div>
  <button>Sign Up</button>
</header>

<style>
  .header {
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 0.5rem 1.2rem;
    box-shadow: 10px 0px 5px 1px rgba(0, 2, 0, 0.8);
    border-radius: 0 5px 5px 0;
  }
  .navigation {
    display: flex;
    align-items: center;
    justify-content: space-between;
    gap: 0.7rem;
  }
  .nav-links {
    text-decoration: none;
  }
  button {
    background-color: transparent;
    cursor: pointer;
    outline: none;
    border: 0.2px solid black;
    padding: 4px 9px;
    font-size: 0.97rem;
    font-weight: 800;
  }
  button:hover {
    transition: all 700ms;
    border-radius: 10px;
  }
</style>
