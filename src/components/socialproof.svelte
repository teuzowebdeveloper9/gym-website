<script>
  import SectionWrapper from "./SectionWrapper.svelte";

  const reviews = [
    {
      id: 1,
      name: "Sarah Johnson",
      comment:
        "Great gym! The equipment is always clean and the staff is super friendly.",
      rating: 5,
    },
    {
      id: 2,
      name: "Michael Smith",
      comment:
        "Good value for the price. I love the group classes and trainers.",
      rating: 4,
    },
    {
      id: 3,
      name: "Emily Davis",
      comment: "Nice facilities but it gets crowded in the evenings.",
      rating: 3,
    },
    {
      id: 4,
      name: "Daniel Wilson",
      comment: "Best gym in town! Amazing atmosphere and modern machines.",
      rating: 5,
    },
    {
      id: 5,
      name: "Olivia Brown",
      comment:
        "Friendly staff, clean locker rooms, and lots of workout options.",
      rating: 4,
    },
  ];
</script>

<SectionWrapper id="socialproof">
  <div
    class="flex-1 flex-col gap-10 sm:gap-14 md:gap-24 py-20 flex items-center justify-center"
  >
    <div class="flex flex-col gap-2">
      <p class="opacity-60 text-base sm:text-lg md:text-xl text-center">
        in case our words are not enough:
      </p>
      <h3
        class="text-4xl sm:text-5xl md:text-6xl max-w-[1000px] mx-auto w-full font-semibold text-center"
      >
        see how our customers <span class="text-orange-400"
          >approve our work</span
        >
      </h3>
      {#each reviews as review}
        <div class="p-4 border-b">
          <h3 class="font-bold">{review.name}</h3>
          <p class="text-sm text-gray-600">{review.comment}</p>
          <p class="text-yellow-400">Rating: {review.rating} ⭐</p>
        </div>
      {/each}
    </div>
  </div>
</SectionWrapper>
