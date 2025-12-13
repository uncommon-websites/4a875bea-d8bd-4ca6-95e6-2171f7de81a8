<script lang="ts">
  const stats = [
    {
      label: "CPD Accredited",
      desc: "Track Limits qualifies for medical continuous professional development credits. This isn't just an experience—it's recognized professional development that counts toward your CPD requirements while delivering transformative leadership insights.",
      img: "/generated/image-professional-medical-conference-setting--1765589084122-7.webp"
    },
    {
      label: "12 Participants Maximum",
      desc: "We deliberately keep groups small to ensure personalized attention and meaningful connections. With a 3:1 participant-to-coach ratio, you'll receive individual guidance throughout both days of the experience.",
      img: "/generated/image-group-of-professional-doctors-in-a-moder-1765589068252-1.webp"
    },
    {
      label: "Porsche Experience Centre",
      desc: "Day two takes place at a world-class Porsche Experience Centre with professional racing coaches. You'll drive high-performance Porsches on a purpose-built track designed to push your limits in a safe, controlled environment.",
      img: "/generated/image-porsche-sports-car-taking-a-sharp-corner-1765589073708-3.webp"
    },
    {
      label: "2-Day Immersion",
      desc: "This isn't a half-day workshop. Track Limits is a complete two-day immersive experience that gives you time to truly explore, reflect, and integrate new leadership capabilities. Day one focuses on skills; day two on application.",
      img: "/generated/image-mid-career-doctor-in-their-40s-reflectin-1765589078658-5.webp"
    }
  ];
</script>

<section class="py-24 px-6 md:px-12 bg-white border-t border-gray-100">
  <div class="mb-16">
    <p class="text-gray-500 max-w-xl">
      What makes Track Limits different? Here's what you need to know about this unique leadership experience.
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
