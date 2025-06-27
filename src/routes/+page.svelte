<script>
  let { children } = $props();
  import "../app.css";
  import Apresentation from "../components/Apresentation.svelte";
  import Footer from "../components/Footer.svelte";
  import Hero from "../components/Hero.svelte";
</script>

<main class="flex flex-col">
  <Hero />
  <Apresentation />
</main>
<Footer />
