<script>
  import Navbar from "../UI/Navbar.svelte";
  import Footer from "../UI/Footer.svelte";
  import AboutInfo from "../components/About/AboutInfo.svelte";
  import Testimonials from "../components/About/Testimonials.svelte";
</script>
<svelte:head>
<title>Hakkımızda | Svelte Hotel</title>
</svelte:head>
<main>
  <Navbar />
  <AboutInfo/>
  <Testimonials/>
  <Footer>Hotel Svelte &copy; 2020 Tüm Hakları Saklıdır.</Footer>
</main>
