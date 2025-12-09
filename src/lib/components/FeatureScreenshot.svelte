<script lang="ts">
  export let title = "";
  export let subtitle = "";
  export let imageSrc = "";
  export let imageAlt = "App screenshot";
  export let align = "center"; // center, left, right (though screenshot mostly shows center or alternating)
  // Actually the screenshot shows large centered texts with large centered images below them.
</script>

<section class="py-20 bg-white">
  <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 text-center">
    <h2 class="text-4xl md:text-5xl font-serif font-medium text-gray-900 mb-6 tracking-tight">{title}</h2>
    {#if subtitle}
      <p class="text-lg text-gray-600 max-w-2xl mx-auto mb-12 leading-relaxed">{subtitle}</p>
    {/if}
    
    <div class="relative rounded-xl overflow-hidden shadow-2xl border border-gray-200 bg-gray-50 p-2 md:p-4">
        <!-- Browser/App Chrome -->
        <!-- <div class="absolute top-0 left-0 right-0 h-8 bg-white border-b border-gray-200 flex items-center px-4 gap-2">
            <div class="w-3 h-3 rounded-full bg-red-400"></div>
            <div class="w-3 h-3 rounded-full bg-yellow-400"></div>
            <div class="w-3 h-3 rounded-full bg-green-400"></div>
        </div> -->
        <!-- Placeholder for the actual complex UI screenshot -->
        <div class="bg-white rounded-lg overflow-hidden min-h-[400px] md:min-h-[600px] flex items-center justify-center relative">
            {#if imageSrc}
                <img src={imageSrc} alt={imageAlt} class="w-full h-auto" />
            {:else}
                <div class="text-gray-400 font-medium">App Screenshot Placeholder</div>
                <!-- We will try to construct a CSS-based mock for the first one at least -->
                <slot />
            {/if}
        </div>
    </div>
  </div>
</section>
