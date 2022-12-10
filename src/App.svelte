<script lang="ts">
  import Header from "./lib/Header.svelte";
  import Nav from "./lib/Nav.svelte";
  import About from "./pages/About.svelte";
  import Contact from "./pages/Contact.svelte";
  import Donate from "./pages/Donate.svelte";
  import Home from "./pages/Home.svelte";
  import Router from 'svelte-spa-router'
  import Carousel from "./lib/carousel.svelte";
  import Footer from "./lib/Footer.svelte";
  const routes = {
    '/': Home,
    '/contact': Contact,
    '/donate': Donate
  }
</script>

<main class="relative overflow-x-hidden">
  
  <Header/>

  <div class="px-[8rem] md:px-4">
    <Nav/>
    <div class="mt-[8rem]">
      <Router {routes} />
    </div>
  </div>
  <Carousel/>
  <Footer />

</main>

<style>
 
</style>