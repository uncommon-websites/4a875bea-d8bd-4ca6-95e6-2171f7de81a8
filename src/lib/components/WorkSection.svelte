<script lang="ts">
  const programDays = [
    {
      day: "Day One",
      title: "Exploring Your Limits",
      desc: "Leadership fundamentals and core skills doctors rarely develop in traditional medical training.",
      bg: "bg-white",
      img: "/generated/image-group-of-professional-doctors-in-a-moder-1765589068252-1.webp",
      dark: false
    },
    {
      day: "Day One",
      title: "Performance Under Pressure",
      desc: "Understanding decision-making, communication, and resilience in high-stakes environments.",
      bg: "bg-gray-100",
      img: "/generated/image-professional-medical-conference-setting--1765589084122-7.webp",
      dark: false
    },
    {
      day: "Day Two",
      title: "Courage & Risk",
      desc: "Translating leadership theory into visceral experience through high-performance driving.",
      bg: "bg-black",
      img: "/generated/image-close-up-of-hands-on-a-porsche-steering--1765589071034-2.webp",
      dark: true
    },
    {
      day: "Day Two",
      title: "Speed & Skill",
      desc: "Professional Porsche coaches guide you through precision driving at full speed on the track.",
      bg: "bg-gray-900",
      img: "/generated/image-porsche-sports-car-taking-a-sharp-corner-1765589073708-3.webp",
      dark: true
    },
    {
      day: "Beyond",
      title: "One-to-One Coaching",
      desc: "Continue your leadership journey with personalized coaching tailored to your goals.",
      bg: "bg-gray-50",
      img: "/generated/image-professional-porsche-driving-instructor--1765589076177-4.webp",
      dark: false,
      full: true
    }
  ];
</script>

<section class="px-6 md:px-12 py-24 bg-white">
  <div class="max-w-3xl mb-16">
    <h2 class="text-2xl md:text-3xl font-medium leading-tight">
      <span class="font-bold">Two days that challenge everything you know about leadership.</span> From the boardroom to the racetrack, discover what you're truly capable of when you push beyond your limits.
    </h2>
  </div>

  <div class="grid grid-cols-1 md:grid-cols-2 gap-x-6 gap-y-12">
    {#each programDays as program}
      <div class="group cursor-pointer {program.full ? 'md:col-span-2' : ''}">
        <div class={`aspect-[4/3] w-full rounded-lg overflow-hidden relative ${program.bg} mb-4 ${program.full ? 'md:aspect-[2.5/1]' : ''}`}>
          {#if program.img}
             <img src={program.img} alt={program.title} class="w-full h-full object-cover transition-transform duration-500 group-hover:scale-105" />
          {:else}
             <div class="w-full h-full flex items-center justify-center">
                <span class={`text-2xl font-bold ${program.dark ? 'text-white' : 'text-black'}`}>{program.title}</span>
             </div>
          {/if}
        </div>
        <div class="flex items-center gap-2 mb-1">
          <span class="text-xs font-bold text-primary-600">{program.day}</span>
          <span class="text-xs text-gray-400">•</span>
          <h3 class="text-sm font-bold">{program.title}</h3>
        </div>
        <p class="text-sm text-gray-600">{program.desc}</p>
      </div>
    {/each}
  </div>
</section>
