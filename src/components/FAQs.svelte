<script>
  import SectionWrapper from "./SectionWrapper.svelte";
  import { faqs } from "../utils/faqs";
</script>

<SectionWrapper id="FAQs">
  <div
    class="flex flex-col items-center justify-center py-12 px-4 max-w-4xl mx-auto"
  >
    <h2 class="text-4xl md:text-5xl font-bold text-center mb-8">
      Frequently Asked <span class="text-orange-400">Questions</span>
    </h2>

    <div class="w-full space-y-6">
      {#each faqs as faq}
        <div class="p-4 border-b border-gray-200">
          <h3 class="text-xl font-semibold mb-2 text-gray-800">
            {faq.question}
          </h3>
          <p class="text-gray-600">{faq.answer}</p>
        </div>
      {/each}
    </div>
  </div>
</SectionWrapper>
