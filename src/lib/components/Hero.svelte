<script lang="ts">
  // Platform and community logos
  const logos = [
    "Ableton",
    "FL Studio",
    "Logic Pro",
    "Splice",
    "Beatport"
  ];
</script>

<section class="relative min-h-screen flex flex-col justify-end pb-20 px-6 md:px-12 bg-gradient-to-b from-black via-gray-900 to-white text-[#1a1a1a]">
  <!-- Gradient overlay with subtle primary color accent -->
  <div class="absolute inset-0 z-[-1] bg-[linear-gradient(180deg,#000_0%,#0a0a0a_30%,#1a1a1a_50%,#f5f5f5_85%,#fff_100%)]"></div>

  <div class="max-w-4xl mb-32 pt-40">
    <h1 class="text-3xl md:text-5xl font-medium leading-[1.15] tracking-tight text-white">
      From Bedroom Producer to Professional Artist. <span class="text-gray-400">Master arrangement fundamentals, overcome creative blocks, and finally finish tracks that get released—with structured courses taught by working producers.</span>
    </h1>
  </div>

  <div class="border-t border-gray-700 pt-8 flex flex-wrap gap-8 md:gap-16 items-center opacity-60 grayscale">
    {#each logos as logo}
      <div class="h-8 flex items-center justify-center font-bold text-xl text-gray-500">{logo}</div>
    {/each}
    <!-- Add more specific logo placeholders if needed -->
    <div class="h-8 w-20 bg-gray-400/20 rounded"></div>
    <div class="h-8 w-20 bg-gray-400/20 rounded"></div>
    <div class="h-8 w-20 bg-gray-400/20 rounded"></div>
  </div>
</section>
