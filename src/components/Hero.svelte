<script>
  import SectionWrapper from "./SectionWrapper.svelte";
  import Header from "./Header.svelte";
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
        class="text-orange-400 italic">be better</span
      >
    </p>
  </div>
</SectionWrapper>
