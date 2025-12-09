<script lang="ts">
  const stats = [
    { label: "Files analyzed", value: "14M" },
    { label: "Citations generated", value: "530K" },
    { label: "Answers generated", value: "27M" },
    { label: "Hours saved per paper", value: "20H" }
  ];
</script>

<section class="py-24 bg-white">
  <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
    <div class="text-center mb-16">
      <h2 class="text-4xl md:text-5xl font-serif font-medium text-gray-900">Trusted by millions</h2>
    </div>

    <div class="grid grid-cols-2 md:grid-cols-4 gap-4">
      {#each stats as stat}
        <div class="bg-gray-50 rounded-xl p-8 text-left h-48 flex flex-col justify-between">
          <span class="text-sm text-gray-500 font-medium">{stat.label}</span>
          <span class="text-4xl md:text-5xl font-medium text-gray-900 tracking-tight">{stat.value}</span>
        </div>
      {/each}
    </div>
  </div>
</section>
