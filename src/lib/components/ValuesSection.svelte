<script lang="ts">
  const photos = [
    {
      title: "Your Creative Space",
      desc: "Learn production in an environment that inspires creativity—whether it's your bedroom studio or our online community.",
      img: "/generated/image-a-bedroom-producers-workspace-with-midi--1765518212947-7.webp"
    },
    {
      title: "Deep Focus",
      desc: "We teach you to enter flow states where your best work happens, moving beyond technical overwhelm into pure creative expression.",
      img: "/generated/image-a-producer-wearing-headphones-eyes-close-1765518217097-8.webp"
    },
    {
      title: "Technical Mastery",
      desc: "Master your DAW and tools so they become invisible—freeing you to focus on the music, not the software.",
      img: "/generated/image-a-laptop-screen-showing-a-digital-audio--1765518221244-9.webp"
    }
  ];
</script>

<section class="py-24 px-6 md:px-12 bg-white">
  <div class="max-w-xl mb-16">
    <h3 class="text-lg font-bold mb-2">We focus on finishing tracks, not collecting tutorials.</h3>
    <p class="text-gray-500 text-sm leading-relaxed">
      In a world of endless YouTube videos and plugin reviews, we provide structured learning paths that actually lead to completed music. Our approach is built on proven workflows, creative systems, and a supportive community that celebrates your releases.
    </p>
  </div>

  <div class="grid grid-cols-1 md:grid-cols-3 gap-6">
    {#each photos as photo}
      <div>
        <div class="aspect-[3/4] rounded-lg overflow-hidden mb-4 bg-gray-100">
          <img src={photo.img} alt={photo.title} class="w-full h-full object-cover" />
        </div>
        <h4 class="text-xs font-bold mb-1">{photo.title}</h4>
        <p class="text-[10px] text-gray-500 leading-relaxed">{photo.desc}</p>
      </div>
    {/each}
  </div>
</section>
