<script>
  let { children } = $props();
  import "../app.css";
  import Apresentation from "../components/Apresentation.svelte";
  import FaQs from "../components/FAQs.svelte";
  import Footer from "../components/Footer.svelte";
  import Hero from "../components/Hero.svelte";
  import Socialproof from "../components/Socialproof.svelte";
  import { openModal } from "$lib";
</script>

{#if $openModal}
  <div
    class="fixed top-0 left-0 w-screen h-screen bg-gray-800 z-50 flex flex-col p-5 px-8"
  >
    <div class="flex items-center justify-between gap-4 border-b pb-2">
      <a href="/">
        <h1 class="text-3xl font-extrabold">
          teuzo <span class="text-orange-400">gym</span>
        </h1>
      </a>
      <button
        on:click={() => ($openModal = false)}
        class="outline-none border-none"
      >
        <i class="fa-solid fa-xmark text-2xl"></i>
      </button>
    </div>

    <!-- Links de navegação no modal -->
    <nav class="flex flex-col gap-6 mt-8">
      <a
        href="#Apresentation"
        on:click={() => ($openModal = false)}
        class="text-lg font-semibold text-gray-600 hover:text-orange-400 transition-colors"
      >
        product
      </a>
      <a
        href="#socialproof"
        on:click={() => ($openModal = false)}
        class="text-lg font-semibold text-gray-600 hover:text-orange-400 transition-colors"
      >
        social proof
      </a>
      <a
        href="#FAQs"
        on:click={() => ($openModal = false)}
        class="text-lg font-semibold text-gray-600 hover:text-orange-400 transition-colors"
      >
        FAQ
      </a>
      <button
        class="text-lg border-2 border-gray-200 hover:bg-amber-300 flex items-center justify-center w-[140px] p-4 rounded-3xl font-semibold text-gray-600 hover:text-orange-400 transition-colors"
      >
        start free
      </button>
    </nav>
  </div>
{/if}
<div
  class="hidden top-0 left-0 w-screen h-screen border-b bg-white z-50 flex flex-col gap-8 p-5 px-8"
>
  <div class="flex items-center justify-between gap-4 border-b pb-2">
    <a href="/">
      <h1 class="text-3xl font-extrabold">
        teuzo <span class="text-orange-400">gym </span>
      </h1>
    </a>
    <button
      on:click={() => ($openModal = false)}
      class="outline-none border-none"
    >
      <i class="fa-solid fa-xmark text-2xl"></i>
    </button>
  </div>
</div>

<main class="flex flex-col">
  <Hero />
  <Apresentation />
  <Socialproof />
  <FaQs />
</main>
<Footer />
