<script lang="ts">
  const testimonials = [
    {
      title: "Dr. Sarah Mitchell",
      role: "Consultant Cardiologist",
      desc: "Track Limits completely changed how I approach leadership in my department. The driving experience wasn't just thrilling—it was a powerful metaphor for decision-making under pressure.",
      img: "/generated/image-mid-career-doctor-in-their-40s-reflectin-1765589078658-5.webp"
    },
    {
      title: "Dr. James Chen",
      role: "Emergency Medicine Director",
      desc: "I've done countless CPD courses, but nothing compares to this. The combination of practical leadership skills and the track experience created insights I couldn't have gained any other way.",
      img: "/generated/image-professional-doctor-in-their-40s-standin-1765589064374-0.webp"
    },
    {
      title: "Dr. Aisha Patel",
      role: "Surgical Consultant",
      desc: "The small group size meant real conversations and genuine connections. I left with not just new skills, but a network of peers who understand the unique challenges of medical leadership.",
      img: "/generated/image-group-of-professional-doctors-in-a-moder-1765589068252-1.webp"
    }
  ];
</script>

<section class="py-24 px-6 md:px-12 bg-white">
  <div class="max-w-xl mb-16">
    <h3 class="text-lg font-bold mb-2">What participants say about Track Limits</h3>
    <p class="text-gray-500 text-sm leading-relaxed">
      Don't just take our word for it. Here's what doctors who've experienced Track Limits have to say about how it transformed their approach to leadership.
    </p>
  </div>

  <div class="grid grid-cols-1 md:grid-cols-3 gap-6">
    {#each testimonials as testimonial}
      <div>
        <div class="aspect-[3/4] rounded-lg overflow-hidden mb-4 bg-gray-100">
          <img src={testimonial.img} alt={testimonial.title} class="w-full h-full object-cover" />
        </div>
        <h4 class="text-xs font-bold mb-1">{testimonial.title}</h4>
        <p class="text-[10px] text-primary-600 mb-2">{testimonial.role}</p>
        <p class="text-[11px] text-gray-600 leading-relaxed italic">"{testimonial.desc}"</p>
      </div>
    {/each}
  </div>
</section>
