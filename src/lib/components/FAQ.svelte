<script lang="ts">
  let openIndex: number | null = null;

  const faqs = [
    { q: "Is Anara free to try?", a: "Yes, Anara offers a free tier that allows you to explore the platform and its core features." },
    { q: "Will this affect my ability to conduct independent research?", a: "Anara is designed to assist, not replace, your critical thinking. It helps organize and retrieve information, but the analysis and conclusions remain yours." },
    { q: "How can I verify the accuracy of AI-generated responses?", a: "Every response from Anara includes citations linked directly to the source text in your uploaded documents, allowing for easy verification." },
    { q: "How secure is my data with Anara?", a: "We take data security seriously. Your data is encrypted and stored securely. We do not use your private data to train our public models without your consent." },
    { q: "What file types does Anara support?", a: "Anara supports PDF, Word documents, and plain text files. We are constantly adding support for more formats." },
    { q: "What is your refund policy?", a: "We offer a 30-day money-back guarantee if you are not satisfied with our premium plans." }
  ];

  function toggle(index: number) {
    openIndex = openIndex === index ? null : index;
  }
</script>

<section class="py-24 bg-white">
  <div class="max-w-3xl mx-auto px-4 sm:px-6 lg:px-8">
    <div class="flex flex-col md:flex-row md:justify-between md:items-start gap-12">
        <div class="md:w-1/3">
            <h2 class="text-4xl font-serif font-medium text-gray-900 leading-tight">Frequently Asked Questions</h2>
        </div>
        
        <div class="md:w-2/3 w-full">
            <div class="space-y-4">
            {#each faqs as faq, i}
                <div class="border-b border-gray-100 pb-4">
                <button 
                    class="w-full text-left flex justify-between items-center py-2 focus:outline-none group"
                    on:click={() => toggle(i)}
                >
                    <span class="text-sm font-medium text-gray-900 group-hover:text-gray-600 transition-colors">{faq.q}</span>
                    <span class="text-xl font-light text-gray-400 ml-4">{openIndex === i ? '−' : '+'}</span>
                </button>
                {#if openIndex === i}
                    <div class="mt-2 text-sm text-gray-600 leading-relaxed pb-2">
                    {faq.a}
                    </div>
                {/if}
                </div>
            {/each}
            </div>
            <div class="mt-8">
                <a href="/faqs" class="text-sm font-medium text-black hover:underline flex items-center gap-1">
                    More FAQs <span class="text-xs">-></span>
                </a>
            </div>
        </div>
    </div>
  </div>
</section>
