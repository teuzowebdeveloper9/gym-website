<script>
  import SectionWrapper from "./SectionWrapper.svelte";
  import Header from "./Header.svelte";
  import CtAs from "./CTAs.svelte";
  export let rating = 5;
</script>

<SectionWrapper id="hero">
  <Header />
  <div
    class="flex flex-col gap-8 flex-1 items-center justify-center pb-10 md:pb-14"
  >
    <h2
      class="text-5xl font-semibold sm:text-6xl md:text-7xl lg:text-8xl max-w-[1200px] mx-auto w-full text-center"
    >
      <span class="text-orange-400">THE</span><span class="text-gray-600"
        >GYM OF THE <span class="text-orange-400">CHAMPIONS</span></span
      >
    </h2>
    <p
      class="text-xl sm:text-2xl md:text-3xl text-center max-w-[1000px] w-full mx-auto"
    >
      to be the best you need to be with the best <span
        class="text-orange-400 italic">be better.</span
      >
    </p>
    <CtAs />
    <div class="flex items-center justify-center text-base gap-2">
      <p>5.0</p>
      {#each [0, 1, 2, 3, 4] as index}
        <div class="grid place-items-center relative">
          <i class="fa-solid fa-star text-gray-300"></i>
          {#if index < rating}
            <i class="fa-solid fa-star text-yellow-400 absolute top-0 left-0"
            ></i>
          {/if}
        </div>
      {/each}
    </div>
  </div>
</SectionWrapper>
