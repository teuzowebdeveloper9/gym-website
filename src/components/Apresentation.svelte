<script>
  import SectionWrapper from "./SectionWrapper.svelte";
  import { feautures } from "../utils/feautures";
</script>

<SectionWrapper id="Apresentation">
  <div class="flex flex-col items-center justify-center gap-8 py-10">
    <h2 class="text-4xl font-bold text-center text-gray-800">Our Features</h2>
    <p class="text-lg text-center text-gray-600 max-w-2xl">
      We offer a range of features to help you achieve your fitness goals.
    </p>
    <div class="grid grid-cols-1 md:grid-cols-3 gap-6 max-w-[1200px] w-full">
      {#each feautures as feature}
        <div
          class="bg-white p-6 rounded-lg shadow-md hover:shadow-lg transition-shadow duration-300"
        >
          <h3 class="text-xl font-semibold text-gray-800 mb-2">
            {feature.title}
          </h3>
          <p class="text-gray-600">{feature.description}</p>
        </div>
      {/each}
    </div>
  </div>
</SectionWrapper>
