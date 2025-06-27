<script>
  let { children } = $props();
  import "../app.css";
  import Footer from "../components/Footer.svelte";
  import Hero from "../components/Hero.svelte";
</script>

<main class="flex flex-col">
  <Hero />
</main>
<Footer />
