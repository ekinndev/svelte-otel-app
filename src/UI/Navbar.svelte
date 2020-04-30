<script>
  import Button from "./Button.svelte";
  import HomeShowcase from "../components/Home/HomeShowcase.svelte";
  import NavbarButton from "./NavbarButton.svelte";
  export let showCase = false;
</script>

<style>
  #navbar {
    background-color: #333;
    color: #fff;
    overflow: hidden;
  }

  #navbar .logo {
    float: left;
  }
  h1 {
    padding: 0;
    margin: 0;
  }

  #navbar ul {
    list-style: none;
    float: right;
  }
  #navbar ul li {
    float: left;
  }
</style>

<header>
  <nav id="navbar">
    <div class="container">
      <h1 class="logo">
        <NavbarButton href="anasayfa">Svelte Hostel</NavbarButton>
      </h1>
      <ul>
        <li>
          <NavbarButton href="anasayfa" isCurrent={true}>
            Anasayfa
          </NavbarButton>
        </li>
        <li>
          <NavbarButton href="hakkimizda">Hakkımızda</NavbarButton>
        </li>
        <li>
          <NavbarButton href="iletisim">İletişim</NavbarButton>
        </li>
      </ul>
    </div>

  </nav>
  {#if showCase}
    <HomeShowcase />
  {/if}
</header>
