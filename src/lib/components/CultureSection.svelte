<script lang="ts">
  const cards = [
    {
      title: "Not Another Conference...",
      subtitle: "An Experience That Changes You.",
      image: "/generated/image-diverse-group-of-doctors-in-racing-suits-1765589081528-6.webp"
    },
    {
      title: "Not Just Theory...",
      subtitle: "Visceral, Unforgettable Learning.",
      image: "/generated/image-close-up-of-hands-on-a-porsche-steering--1765589071034-2.webp"
    },
    {
      title: "Not Generic CPD...",
      subtitle: "Leadership Development That Matters.",
      image: "/generated/image-professional-porsche-driving-instructor--1765589076177-4.webp"
    }
  ];
</script>

<section class="py-24 px-6 md:px-12 bg-white">
  <div class="max-w-2xl mb-16">
    <p class="text-xl md:text-2xl leading-relaxed text-gray-800">
      Track Limits isn't traditional professional development. It's an immersive experience that combines world-class leadership training with the thrill of high-performance driving—designed specifically for doctors who want more from their CPD.
    </p>
  </div>

  <div class="grid grid-cols-1 md:grid-cols-3 gap-6">
    {#each cards as card}
      <div class="group">
        <div class="aspect-[4/3] overflow-hidden rounded-lg mb-4 bg-gray-100">
          <img src={card.image} alt={card.title} class="w-full h-full object-cover group-hover:scale-105 transition-all duration-500" />
        </div>
        <h3 class="text-sm text-gray-500 mb-1">{card.title}</h3>
        <p class="text-sm font-bold">{card.subtitle}</p>
        
        <div class="flex justify-between mt-4 text-xs text-gray-400">
           <span>Track Limits</span>
           <span>→</span>
        </div>
      </div>
    {/each}
  </div>
</section>
