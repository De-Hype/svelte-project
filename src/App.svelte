<script>
  import Footer from "./lib/Components/Footer.svelte";
  import Header from "./lib/Components/Header.svelte";
  import Hero from "./lib/Components/Hero.svelte";
  import Pricing from "./lib/Components/Pricing.svelte";
  import Testimony from "./lib/Components/Testimony.svelte";
</script>

<main>
  <Header />
  <Hero />
  <Pricing />
  <Testimony />
  <Footer />
</main>

<style>
  main {
    min-height: 100vh;
  }
</style>
