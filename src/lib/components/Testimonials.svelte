<script lang="ts">
  const testimonials = [
    { name: "Anne", role: "Research Scientist, GSK", text: "I love it! It accomplishes in minutes what would take me ages to do manually. What really impresses me is how Anara recognizes themes and patterns I've completely missed. It's particularly good at pointing out important details and research gaps that aren't immediately obvious." },
    { name: "Filip", role: "Data Scientist, Intel", text: "I've tried a lot of AI research apps, and Anara is so far ahead in simplicity, quality, and speed!" },
    { name: "Zeyu", role: "Lab Assistant, UC Berkeley", text: "I'm using Anara right now for my research into single-cell multiomics frameworks, and it's amazing!" },
    { name: "Paul", role: "Research Scientist, Biogen", text: "With Anara, I'm able to do in 30 mins what used to take 3 hours. There's nothing else like it." },
    { name: "Alice", role: "Associate, Goldman Sachs", text: "Genuinely makes research so much more intuitive. The related documents feature is amazing, and I love how effortless the annotation process is." },
    { name: "Ethan", role: "Senior Scientist, Roche", text: "I'm very impressed. Delighted by the tool you made... It's reassuring when we have the citations." },
    { name: "Samantha", role: "Neuroscientist, NIH", text: "Anara makes life easier for anyone new to the team. It breaks down complex information so effectively that newcomers can contribute and feel included right from the start." },
    { name: "Michael", role: "Physician, Cedars Sinai", text: "Interacting with documents on Anara is like speaking to the team who wrote the research paper. It's fantastic." },
    { name: "Nabila", role: "Undergraduate Student, MIT", text: "It aided in my research works tremendously... The review writing that would take me several days now it's only a matter of minutes!!! I already recommended it to all my friends struggling with research papers." },
    { name: "Jeremy", role: "Research Assistant, PwC", text: "This website is simply awesome. Every researcher should employ it to help and ease their work." },
    { name: "Zevarn", role: "Physician, Kaiser Permanente", text: "I love how functional and flexible it is for understanding papers. It provides a unified platform for reading, writing, and referencing, plus the search features help you explore concepts easily. It makes the whole process of working with academic papers so much smoother." },
    { name: "Elyane", role: "Astrophysicle Physicist", text: "It's so useful to be able to find a little piece of information you know you've already read in a paper but you don't remember where. And it's trustworthy since it show you where it picked it's information, and you can verify afterward." },
    { name: "Taylor", role: "Master's Student, Columbia University", text: "Excellent tool to use, especially for understanding and translating research papers. I'm enjoying it. Thank you" },
    { name: "Joy", role: "Med Student, Yale University", text: "I'm a medical student and I use Anara to summarize clinical guidelines. It's a lifesaver." },
    { name: "Sofia", role: "PhD Student, Stanford University", text: "As a PhD candidate, Anara is my number one app for annotations, lit reviews and manuscripts." },
    { name: "Alamin", role: "Dermatologist, Mayo Clinic", text: "Anara makes diving into research papers so much easier and quicker. A must-try tool." }
  ];
</script>

<section class="py-24 bg-white">
  <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
    <div class="text-center mb-16">
      <h2 class="text-4xl md:text-5xl font-serif font-medium text-gray-900">What people are saying</h2>
    </div>

    <!-- Masonry-like grid using columns -->
    <div class="columns-1 md:columns-2 lg:columns-4 gap-6 space-y-6">
      {#each testimonials as t}
        <div class="break-inside-avoid bg-gray-50 rounded-xl p-6">
          <div class="mb-4">
            <h4 class="text-sm font-bold text-gray-900">{t.name}</h4>
            <p class="text-xs text-gray-500">{t.role}</p>
          </div>
          <p class="text-sm text-gray-700 leading-relaxed">"{t.text}"</p>
        </div>
      {/each}
    </div>
    
    <!-- Fade out effect at bottom if needed, but screenshot shows full list or at least a lot of them. 
         The screenshot shows a fade at the very bottom. -->
    <div class="h-32 bg-gradient-to-t from-white to-transparent -mt-32 relative z-10 pointer-events-none"></div>
  </div>
</section>
