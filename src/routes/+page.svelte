<script>
  let { children } = $props();
  import "../app.css";
  import Apresentation from "../components/Apresentation.svelte";
  import Footer from "../components/Footer.svelte";
  import Hero from "../components/Hero.svelte";
  import Socialproof from "../components/Socialproof.svelte";
</script>

<main class="flex flex-col">
  <Hero />
  <Apresentation />
  <Socialproof />
</main>
<Footer />
