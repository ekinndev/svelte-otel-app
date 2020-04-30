<script>
  import Button from "./Button.svelte";
  import HomeShowcase from "../components/Home/HomeShowcase.svelte";
  import NavbarButton from "./NavbarButton.svelte";
  import { getContext } from "svelte";
  import { ROUTER } from "svelte-routing/src/contexts";
  const { activeRoute } = getContext(ROUTER);
  export let showCase = false;
  let anasayfaMi = false;
  let hakkimizdaMi = false;
  let iletisimMi = false;
  $: if (
    $activeRoute.route.path == "/" ||
    $activeRoute.route.path == "anasayfa/"
  ) {
    anasayfaMi = true;
  } else if ($activeRoute.route.path == "hakkimizda/") {
    hakkimizdaMi = true;
  } else if ($activeRoute.route.path == "iletisim/") {
    iletisimMi = true;
  }
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
        <NavbarButton href="anasayfa">Svelte Otel</NavbarButton>
      </h1>
      <ul>
        <li>
          <NavbarButton href="anasayfa" isCurrent={anasayfaMi}>
            Anasayfa
          </NavbarButton>
        </li>
        <li>
          <NavbarButton href="hakkimizda" isCurrent={hakkimizdaMi}>
            Hakkımızda
          </NavbarButton>
        </li>
        <li>
          <NavbarButton href="iletisim" isCurrent={iletisimMi}>
            İletişim
          </NavbarButton>
        </li>
      </ul>
    </div>

  </nav>
  {#if showCase}
    <HomeShowcase />
  {/if}
</header>
