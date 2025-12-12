<script lang="ts">
  const projects = [
    {
      client: "Music Production Fundamentals",
      desc: "Master the core concepts every producer needs to know.",
      bg: "bg-black",
      img: "/generated/image-a-focused-young-music-producer-working-o-1765518181997-0.webp",
      dark: true
    },
    {
      client: "Arrangement & Song Structure",
      desc: "Learn to build tracks that keep listeners engaged from start to finish.",
      bg: "bg-gray-200",
      img: "/generated/image-a-confident-music-producer-in-headphones-1765518187400-1.webp",
      dark: false
    },
    {
      client: "Sound Design Mastery",
      desc: "Create unique sounds that define your signature style.",
      bg: "bg-gray-900",
      img: "/generated/image-a-laptop-screen-showing-a-digital-audio--1765518221244-9.webp",
      dark: false
    },
    {
      client: "Mixing & Mastering",
      desc: "Polish your tracks to professional, release-ready quality.",
      bg: "bg-black",
      img: "",
      dark: true
    },
    {
      client: "Creative Workflow Systems",
      desc: "Build habits and systems that help you finish more tracks, faster.",
      bg: "bg-[#f0f0f0]",
      img: "/generated/image-a-bedroom-producers-workspace-with-midi--1765518212947-7.webp",
      dark: false,
      full: true
    },
    {
      client: "Genre-Specific Production",
      desc: "Deep dives into house, techno, bass music, and more.",
      bg: "bg-[#e0e0e0]",
      img: "/generated/image-a-professional-music-producer-performing-1765518191556-2.webp",
      dark: false
    },
    {
      client: "Release Strategy",
      desc: "Navigate labels, distribution, and building your artist brand.",
      bg: "bg-gray-100",
      img: "",
      dark: false
    }
  ];
</script>

<section class="px-6 md:px-12 py-24 bg-white">
  <div class="max-w-3xl mb-16">
    <h2 class="text-2xl md:text-3xl font-medium leading-tight">
      <span class="font-bold">We teach arrangement fundamentals first,</span> helping you overcome gear obsession and technical overwhelm so you can focus on what matters: finishing tracks that showcase your unique sound.
    </h2>
  </div>

  <div class="grid grid-cols-1 md:grid-cols-2 gap-x-6 gap-y-12">
    {#each projects as project}
      <div class="group cursor-pointer {project.full ? 'md:col-span-2' : ''}">
        <div class={`aspect-[4/3] w-full rounded-lg overflow-hidden relative ${project.bg} mb-4 ${project.full ? 'md:aspect-[2.5/1]' : ''}`}>
          {#if project.img}
             <img src={project.img} alt={project.client} class="w-full h-full object-cover transition-transform duration-500 group-hover:scale-105" />
          {:else}
             <!-- Placeholder for course graphics on solid bg -->
             <div class="w-full h-full flex items-center justify-center">
                <span class={`text-2xl font-bold ${project.dark ? 'text-white' : 'text-black'}`}>{project.client}</span>
             </div>
          {/if}
        </div>
        <h3 class="text-sm font-bold mb-1">{project.client}</h3>
        <p class="text-sm text-gray-600">{project.desc}</p>
      </div>
    {/each}
  </div>
</section>
