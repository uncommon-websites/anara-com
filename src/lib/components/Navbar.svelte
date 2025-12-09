<script lang="ts">
  export let sticky = false;
</script>

<nav class="w-full bg-white border-b border-gray-100 py-4 px-6 flex items-center justify-between {sticky ? 'sticky top-0 z-50' : ''}">
  <div class="flex items-center gap-8">
    <a href="/" class="text-xl font-bold font-sans tracking-tight">Anara</a>
    
    <div class="hidden md:flex items-center gap-6 text-sm font-medium text-gray-600">
      <div class="group relative cursor-pointer flex items-center gap-1">
        Use cases
        <svg xmlns="http://www.w3.org/2000/svg" width="12" height="12" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="opacity-50"><path d="m6 9 6 6 6-6"/></svg>
      </div>
      <div class="group relative cursor-pointer flex items-center gap-1">
        Resources
        <svg xmlns="http://www.w3.org/2000/svg" width="12" height="12" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="opacity-50"><path d="m6 9 6 6 6-6"/></svg>
      </div>
      <a href="/pricing" class="hover:text-black">Pricing</a>
      <a href="/careers" class="hover:text-black">Careers</a>
      <a href="/contact" class="hover:text-black">Contact sales</a>
    </div>
  </div>

  <div class="flex items-center gap-4">
    <a href="/login" class="text-sm font-medium text-gray-600 hover:text-black">Log in</a>
    <a href="/signup" class="bg-black text-white text-sm font-medium px-4 py-2 rounded-full hover:bg-gray-800 transition-colors">
      Get Anara free
    </a>
  </div>
</nav>
