<script lang="ts">
  const cards = [
    {
      title: "We're Not Just Teachers...",
      subtitle: "We're Working Producers.",
      image: "/generated/image-a-diverse-group-of-young-producers-colla-1765518195819-3.webp"
    },
    {
      title: "We Don't Just Share Theory...",
      subtitle: "We Show Real Workflows.",
      image: "/generated/image-a-young-producer-having-a-breakthrough-m-1765518200379-4.webp"
    },
    {
      title: "We Don't Just Teach...",
      subtitle: "We Build Community.",
      image: "/generated/image-a-mentor-and-student-reviewing-music-pro-1765518204623-5.webp"
    }
  ];
</script>

<section class="py-24 px-6 md:px-12 bg-white">
  <div class="max-w-2xl mb-16">
    <p class="text-xl md:text-2xl leading-relaxed text-gray-800">
      Learning production isn't about collecting more tutorials—it's about structured guidance from producers who've been where you are. We're here to help you break through creative blocks and finally finish tracks.
    </p>
  </div>

  <div class="grid grid-cols-1 md:grid-cols-3 gap-6">
    {#each cards as card}
      <div class="group">
        <div class="aspect-[4/3] overflow-hidden rounded-lg mb-4 bg-gray-100">
          <img src={card.image} alt={card.title} class="w-full h-full object-cover grayscale group-hover:grayscale-0 transition-all duration-500" />
        </div>
        <h3 class="text-sm text-gray-500 mb-1">{card.title}</h3>
        <p class="text-sm font-bold">{card.subtitle}</p>
        
        <div class="flex justify-between mt-4 text-xs text-gray-400">
           <span>01</span>
           <span>-></span>
        </div>
      </div>
    {/each}
  </div>
</section>
