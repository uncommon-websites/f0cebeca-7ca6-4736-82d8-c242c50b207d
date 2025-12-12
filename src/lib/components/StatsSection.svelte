<script lang="ts">
  const stats = [
    {
      label: "500K+ Students",
      desc: "We're building toward a community of half a million producers worldwide. From bedroom beginners to artists signing their first releases, our students span every level and genre of electronic music production. Join a global network of creators who support each other's growth.",
      img: "/generated/image-a-diverse-group-of-young-producers-colla-1765518195819-3.webp"
    },
    {
      label: "85% Completion Rate",
      desc: "Unlike typical online courses with 5-10% completion rates, our structured curriculum and community support keep students engaged. We focus on finishing tracks, not just watching videos—because completed music is what transforms bedroom producers into artists.",
      img: "/generated/image-a-young-producer-having-a-breakthrough-m-1765518200379-4.webp"
    },
    {
      label: "$4.2B Market",
      desc: "The music education market is massive and growing. We're capturing this opportunity by offering what bedroom producers actually need: practical, arrangement-first training that cuts through gear obsession and gets you making music that matters.",
      img: "/generated/image-a-confident-music-producer-in-headphones-1765518187400-1.webp"
    },
    {
      label: "Producer-Taught",
      desc: "Every course is created and taught by working producers with real releases and industry experience. No academic theory without context—just proven workflows and techniques that actually work in today's music landscape.",
      img: "/generated/image-a-music-producer-teaching-online-speakin-1765518208873-6.webp"
    }
  ];
</script>

<section class="py-24 px-6 md:px-12 bg-white border-t border-gray-100">
  <div class="mb-16">
    <p class="text-gray-500 max-w-xl">
      Curious about our impact? Here's a snapshot of our community, our approach, and the results we're proud of.
    </p>
  </div>

  <div class="space-y-16">
    {#each stats as stat}
      <div class="flex flex-col md:flex-row md:items-start justify-between gap-8 border-b border-gray-100 pb-16 last:border-0">
        <h3 class="text-2xl md:text-4xl font-medium w-full md:w-1/3">{stat.label}</h3>
        <div class="w-full md:w-1/3">
           <p class="text-xs leading-relaxed text-gray-500">{stat.desc}</p>
        </div>
        <div class="w-full md:w-1/6 flex justify-end">
           <img src={stat.img} alt={stat.label} class="w-20 h-20 object-cover rounded bg-gray-100" />
        </div>
      </div>
    {/each}
  </div>
</section>
