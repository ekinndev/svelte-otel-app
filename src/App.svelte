<script>
  import { Router, Link, Route } from "svelte-routing";
  import Home from "./routes/Home.svelte";
  import About from "./routes/About.svelte";
  import Contact from "./routes/Contact.svelte";
</script>

<Router>

  <Route path="/anasayfa"><Home/></Route>


  <Route path="/hakkimizda">
    <About />
  </Route>
  <Route path="/iletisim">
    <Contact />
  </Route>
  <Route path="/">
    <Home />
  </Route>
  <Route path="*">
    404
  </Route>

</Router>
