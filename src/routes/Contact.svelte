<script>
  import Navbar from "../UI/Navbar.svelte";
  import Footer from "../UI/Footer.svelte";
  import ContactInfo from "../components/Contact/ContactInfo.svelte";
  import ContactForm from "../components/Contact/ContactForm.svelte";

</script>
<svelte:head>
<title>İletişim | Svelte Otel</title>
</svelte:head>
<main>
  <Navbar />
  <ContactForm/>
  <ContactInfo/>
  <Footer>Otel Svelte &copy; 2020 Tüm Hakları Saklıdır.</Footer>
</main>
