<script>
  import Navbar from "../UI/Navbar.svelte";
  import HomeInfo from "../components/Home/HomeInfo.svelte";
  import HomeFeature from "../components/Home/HomeFeature.svelte";
  import Footer from "../UI/Footer.svelte";
</script>
<svelte:head>
<title>Anasayfa | Svelte Otel</title>
</svelte:head>
<main>
  <Navbar showCase="{true}"/>
  <HomeInfo />
  <HomeFeature />
  <Footer>Otel Svelte &copy; 2020 Tüm Hakları Saklıdır.</Footer>
</main>
