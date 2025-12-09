<script lang="ts">
  import Navbar from "$lib/components/Navbar.svelte";
  import LogoCloud from "$lib/components/LogoCloud.svelte";
  import FeatureScreenshot from "$lib/components/FeatureScreenshot.svelte";
  import FeatureGrid from "$lib/components/FeatureGrid.svelte";
  import Stats from "$lib/components/Stats.svelte";
  import Testimonials from "$lib/components/Testimonials.svelte";
  import FAQ from "$lib/components/FAQ.svelte";
  import CTA from "$lib/components/CTA.svelte";
  import Footer from "$lib/components/Footer.svelte";
</script>

<Navbar />

<main>
  <!-- Hero Section -->
  <section class="pt-24 pb-12 md:pt-32 md:pb-20 bg-white text-center px-4">
    <h1 class="text-5xl md:text-7xl font-serif font-medium text-gray-900 mb-6 tracking-tight leading-[1.1]">
      AI workspace for scientists,<br />students, and research teams
    </h1>
    <p class="text-lg text-gray-600 max-w-2xl mx-auto mb-10 leading-relaxed">
      Search for papers, extract key passages, organize research and<br class="hidden md:block" />
      write with automatic citations — all without sacrificing academic rigor
    </p>
    <div class="flex flex-col sm:flex-row items-center justify-center gap-4 mb-20">
      <a href="/signup" class="bg-black text-white text-sm font-medium px-6 py-3 rounded-full hover:bg-gray-800 transition-colors w-full sm:w-auto">
        Get Anara free
      </a>
      <a href="/demo" class="bg-gray-100 text-gray-900 text-sm font-medium px-6 py-3 rounded-full hover:bg-gray-200 transition-colors w-full sm:w-auto">
        Request demo
      </a>
    </div>

    <LogoCloud />
  </section>

  <!-- Hero Screenshot -->
  <section class="pb-24 px-4">
    <div class="max-w-7xl mx-auto">
        <div class="relative rounded-xl overflow-hidden shadow-2xl border border-gray-200 bg-gray-50 p-2 md:p-4">
            <div class="bg-white rounded-lg overflow-hidden aspect-[16/9] relative flex flex-col md:flex-row">
                <!-- Left Panel: Flashcards/Quiz -->
                <div class="w-full md:w-1/2 border-r border-gray-100 p-8 flex flex-col justify-center items-center relative">
                    <div class="absolute top-4 left-4 text-xs font-bold text-gray-500">Transformer Model Concepts</div>
                    <div class="absolute top-4 right-4 text-gray-400"><svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><rect x="3" y="3" width="18" height="18" rx="2" ry="2"/><line x1="9" y1="3" x2="9" y2="21"/></svg></div>
                    
                    <div class="w-full max-w-md bg-white rounded-xl shadow-sm border border-gray-200 p-6">
                        <div class="text-xs font-bold text-gray-900 mb-4">Multiple Choice</div>
                        <p class="text-sm text-gray-800 mb-6">What is the main innovation introduced by the Transformer model in 'Attention Is All You Need'?</p>
                        
                        <div class="space-y-3">
                            <div class="flex items-center gap-3 p-3 rounded-lg border border-green-200 bg-green-50">
                                <span class="text-xs font-bold text-green-700">A.</span>
                                <span class="text-xs text-green-800">Using only attention mechanisms, removing recurrence and convolution</span>
                            </div>
                            <div class="flex items-center gap-3 p-3 rounded-lg border border-gray-100 hover:bg-gray-50">
                                <span class="text-xs font-bold text-gray-400">B.</span>
                                <span class="text-xs text-gray-500">Stacking more layers in RNNs</span>
                            </div>
                            <div class="flex items-center gap-3 p-3 rounded-lg border border-gray-100 hover:bg-gray-50">
                                <span class="text-xs font-bold text-gray-400">C.</span>
                                <span class="text-xs text-gray-500">Introducing convolutional layers for sequence modeling</span>
                            </div>
                            <div class="flex items-center gap-3 p-3 rounded-lg border border-gray-100 hover:bg-gray-50">
                                <span class="text-xs font-bold text-gray-400">D.</span>
                                <span class="text-xs text-gray-500">Using only feed-forward networks</span>
                            </div>
                        </div>
                        
                        <div class="mt-6 text-center text-xs text-gray-400">Click to reveal explanation</div>
                    </div>
                    
                    <div class="mt-8 flex items-center gap-4 text-gray-400">
                        <button class="p-2 rounded-full border border-gray-200 hover:bg-gray-50">←</button>
                        <span class="text-xs font-medium">1 / 20</span>
                        <button class="p-2 rounded-full border border-gray-200 hover:bg-gray-50">→</button>
                    </div>
                </div>

                <!-- Right Panel: Chat/Notes -->
                <div class="w-full md:w-1/2 p-6 bg-gray-50/50 flex flex-col border-t md:border-t-0 md:border-l border-gray-100">
                    <div class="flex justify-between items-center mb-6">
                         <div class="flex items-center gap-2">
                            <div class="w-6 h-6 bg-gray-200 rounded-full"></div>
                            <span class="text-xs font-bold text-gray-700">Transformer Model Concepts</span>
                         </div>
                         <div class="text-xs text-gray-400">Source</div>
                    </div>

                    <div class="flex-1 space-y-6">
                        <!-- Message 1 -->
                        <div class="flex gap-3">
                            <div class="w-6 h-6 bg-gray-200 rounded-full flex-shrink-0"></div>
                            <div class="bg-white p-3 rounded-lg border border-gray-100 text-xs text-gray-700 shadow-sm max-w-[90%]">
                                What effect would stacking more layers in RNNs have?
                            </div>
                        </div>

                        <!-- Response 1 -->
                        <div class="flex gap-3">
                            <div class="w-6 h-6 bg-black rounded-full flex-shrink-0 flex items-center justify-center text-white text-[10px]">A</div>
                            <div class="space-y-2 max-w-[90%]">
                                <div class="flex items-center gap-2 text-[10px] text-gray-500">
                                    <span class="flex items-center gap-1"><span class="w-3 h-3 bg-gray-200 rounded-sm"></span> Read Transformer Model Concepts</span>
                                </div>
                                <div class="space-y-1">
                                    <div class="h-2 bg-gray-200 rounded w-full"></div>
                                    <div class="h-2 bg-gray-200 rounded w-5/6"></div>
                                    <div class="h-2 bg-gray-200 rounded w-4/5"></div>
                                </div>
                            </div>
                        </div>
                        
                        <!-- Message 2 -->
                         <div class="flex gap-3 mt-8">
                            <div class="w-6 h-6 bg-gray-200 rounded-full flex-shrink-0"></div>
                            <div class="bg-white p-3 rounded-lg border border-gray-100 text-xs text-gray-700 shadow-sm max-w-[90%]">
                                ...
                            </div>
                        </div>
                    </div>

                    <!-- Input Area -->
                    <div class="mt-4 relative">
                        <input type="text" placeholder="Ask this folder a question..." class="w-full bg-white border border-gray-200 rounded-lg pl-4 pr-10 py-3 text-xs focus:outline-none focus:border-gray-400 shadow-sm" />
                        <div class="absolute right-2 top-2 bottom-2 flex items-center gap-2">
                            <div class="w-6 h-6 bg-gray-100 rounded flex items-center justify-center text-gray-400">↑</div>
                        </div>
                        <div class="absolute left-4 bottom-[-24px] flex gap-2">
                             <span class="text-[10px] bg-blue-50 text-blue-600 px-1.5 py-0.5 rounded">@ Mention</span>
                             <span class="text-[10px] bg-gray-100 text-gray-600 px-1.5 py-0.5 rounded">⚙ GPT 5 ⌄</span>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
  </section>

  <FeatureGrid />

  <!-- Feature: Understand any file -->
  <FeatureScreenshot 
    title="Understand any file or group of files, instantly" 
    subtitle="Whether it's a dense 200-page textbook, a new clinical study, or a technical research paper, just upload it and start asking questions"
  >
     <!-- Mockup for PDF Viewer + Chat -->
     <div class="w-full h-full flex bg-white flex-col md:flex-row">
        <!-- Sidebar -->
        <div class="w-full md:w-64 border-r border-gray-200 p-4 hidden md:flex flex-col gap-4 bg-gray-50/30">
            <div class="flex gap-2 mb-2">
                <div class="w-3 h-3 rounded-full bg-gray-300"></div>
                <div class="w-3 h-3 rounded-full bg-gray-300"></div>
                <div class="w-3 h-3 rounded-full bg-gray-300"></div>
            </div>
            <div class="space-y-2">
                <div class="h-6 bg-gray-100 rounded w-full"></div>
                <div class="h-6 bg-white border border-gray-200 rounded w-full"></div>
                <div class="h-6 bg-white border border-gray-200 rounded w-full"></div>
            </div>
        </div>
        <!-- Main Content: PDF View -->
        <div class="flex-1 p-8 bg-gray-50 overflow-hidden relative min-h-[400px]">
            <div class="bg-white shadow-md w-full h-full rounded mx-auto max-w-3xl p-8 text-[10px] text-gray-400 overflow-hidden">
                <div class="w-full h-4 bg-gray-200 mb-6 rounded"></div>
                <div class="flex gap-4 mb-6">
                    <div class="w-1/2 space-y-2">
                        <div class="h-2 bg-gray-100 rounded w-full"></div>
                        <div class="h-2 bg-gray-100 rounded w-full"></div>
                        <div class="h-2 bg-gray-100 rounded w-5/6"></div>
                        <div class="h-2 bg-gray-100 rounded w-full"></div>
                    </div>
                    <div class="w-1/2 space-y-2">
                        <div class="h-2 bg-gray-100 rounded w-full"></div>
                        <div class="h-2 bg-gray-100 rounded w-full"></div>
                        <div class="h-2 bg-gray-100 rounded w-5/6"></div>
                    </div>
                </div>
                <!-- Table Mockup -->
                <div class="border border-gray-200 rounded p-2 mb-6">
                    <div class="grid grid-cols-4 gap-2 mb-2 border-b border-gray-100 pb-2">
                        <div class="h-2 bg-gray-200 rounded"></div>
                        <div class="h-2 bg-gray-200 rounded"></div>
                        <div class="h-2 bg-gray-200 rounded"></div>
                        <div class="h-2 bg-gray-200 rounded"></div>
                    </div>
                     <div class="grid grid-cols-4 gap-2">
                        <div class="h-2 bg-gray-100 rounded"></div>
                        <div class="h-2 bg-gray-100 rounded"></div>
                        <div class="h-2 bg-gray-100 rounded"></div>
                        <div class="h-2 bg-gray-100 rounded"></div>
                    </div>
                </div>
            </div>
        </div>
        <!-- Right Sidebar: Chat -->
        <div class="w-full md:w-80 border-l border-gray-200 p-4 flex flex-col bg-white">
             <div class="flex items-center gap-2 mb-4 border-b border-gray-100 pb-2">
                <div class="w-4 h-4 bg-gray-200 rounded"></div>
                <span class="text-xs font-bold">Trainable Dynamic Routing</span>
             </div>
             <div class="flex-1 space-y-4">
                 <div class="bg-gray-50 p-3 rounded text-xs text-gray-600">
                    What are the limitations of traditional routing mechanisms in capsule networks?
                 </div>
                 <div class="space-y-2">
                     <div class="h-2 bg-gray-100 rounded w-full"></div>
                     <div class="h-2 bg-gray-100 rounded w-5/6"></div>
                     <div class="h-2 bg-gray-100 rounded w-4/5"></div>
                 </div>
             </div>
             <div class="mt-4">
                <div class="h-10 border border-gray-200 rounded-full w-full"></div>
             </div>
        </div>
     </div>
  </FeatureScreenshot>

  <!-- Feature: Concise answers -->
  <FeatureScreenshot 
    title="Get concise, scholarly answers to any question" 
    subtitle="When you ask a question, Anara searches major academic databases like PubMed, arXiv and JSTOR to deliver a comprehensive response"
  >
    <!-- Mockup for Search/Answer Interface -->
    <div class="w-full h-full bg-white p-8 flex flex-col items-center">
        <div class="w-full max-w-2xl">
            <!-- User Query -->
            <div class="flex justify-end mb-8">
                <div class="bg-gray-100 text-gray-800 p-4 rounded-2xl rounded-tr-sm text-sm max-w-lg">
                    How could integrating HRM's hierarchical planner-executor with Transformer self-attention and the incremental-constraint self-supervised RL method mitigate the reasoning vs. instruction-following trade-off in standard LLMs?
                </div>
            </div>
            
            <!-- AI Response -->
            <div class="flex gap-4">
                <div class="w-8 h-8 bg-black rounded-full flex-shrink-0"></div>
                <div class="flex-1">
                    <div class="flex items-center gap-2 mb-4">
                        <span class="text-xs font-bold text-gray-500 uppercase tracking-wider">Searched web for papers</span>
                        <span class="text-xs text-gray-400">8 results ⌄</span>
                    </div>
                    
                    <div class="grid grid-cols-1 gap-2 mb-6">
                        <div class="flex items-center gap-2 text-xs text-gray-600 border border-gray-100 p-2 rounded hover:bg-gray-50">
                            <span class="w-4 h-4 bg-gray-200 rounded-sm"></span>
                            Hierarchical Reasoning Model - arXiv
                        </div>
                        <div class="flex items-center gap-2 text-xs text-gray-600 border border-gray-100 p-2 rounded hover:bg-gray-50">
                            <span class="w-4 h-4 bg-gray-200 rounded-sm"></span>
                            Hierarchical Neuro-Symbolic Decision Transformer
                        </div>
                        <div class="flex items-center gap-2 text-xs text-gray-600 border border-gray-100 p-2 rounded hover:bg-gray-50">
                            <span class="w-4 h-4 bg-gray-200 rounded-sm"></span>
                            Think Only When You Need with Large Hybrid-Reasoning
                        </div>
                    </div>
                    
                    <div class="space-y-3">
                        <div class="h-3 bg-gray-100 rounded w-full"></div>
                        <div class="h-3 bg-gray-100 rounded w-full"></div>
                        <div class="h-3 bg-gray-100 rounded w-5/6"></div>
                        <div class="h-3 bg-gray-100 rounded w-4/5"></div>
                         <div class="h-3 bg-gray-100 rounded w-full"></div>
                    </div>
                    
                    <div class="flex gap-2 mt-6">
                        <div class="w-6 h-6 rounded bg-gray-100 flex items-center justify-center text-xs text-gray-400">1</div>
                        <div class="w-6 h-6 rounded bg-gray-100 flex items-center justify-center text-xs text-gray-400">2</div>
                    </div>
                </div>
            </div>
        </div>
    </div>
  </FeatureScreenshot>

  <!-- Feature: Flashcards (Reuse Hero Screenshot style) -->
  <FeatureScreenshot 
    title="Generate flashcards and multiple choice questions" 
    subtitle="Upload lecture slides, textbooks, or videos, and Anara will create flashcards and practice quizzes tailored to your specific materials"
  >
     <!-- Reusing the hero structure but maybe simplified or just the left part focused -->
     <div class="w-full h-full bg-gray-50 flex items-center justify-center p-8">
         <div class="bg-white rounded-xl shadow-lg border border-gray-200 p-8 max-w-lg w-full">
            <div class="text-xs font-bold text-gray-900 mb-4">Multiple Choice</div>
            <p class="text-sm text-gray-800 mb-6">What is the main innovation introduced by the Transformer model in 'Attention Is All You Need'?</p>
            
            <div class="space-y-3">
                <div class="flex items-center gap-3 p-3 rounded-lg border border-green-200 bg-green-50">
                    <span class="text-xs font-bold text-green-700">A.</span>
                    <span class="text-xs text-green-800">Using only attention mechanisms, removing recurrence and convolution</span>
                </div>
                <div class="flex items-center gap-3 p-3 rounded-lg border border-gray-100">
                    <span class="text-xs font-bold text-gray-400">B.</span>
                    <span class="text-xs text-gray-500">Stacking more layers in RNNs</span>
                </div>
                <div class="flex items-center gap-3 p-3 rounded-lg border border-gray-100">
                    <span class="text-xs font-bold text-gray-400">C.</span>
                    <span class="text-xs text-gray-500">Introducing convolutional layers for sequence modeling</span>
                </div>
            </div>
            <div class="mt-6 text-center text-xs text-gray-400">Click to reveal explanation</div>
             <div class="mt-8 flex items-center justify-center gap-4 text-gray-400">
                <button class="p-2 rounded-full border border-gray-200 hover:bg-gray-50">←</button>
                <span class="text-xs font-medium">1 / 20</span>
                <button class="p-2 rounded-full border border-gray-200 hover:bg-gray-50">→</button>
            </div>
         </div>
     </div>
  </FeatureScreenshot>

  <!-- Feature: Library -->
  <FeatureScreenshot 
    title="Build a single, searchable library for all your projects" 
    subtitle="Whether working solo or collaborating with a team, Anara provides one organized place for all your scholarly work"
  >
    <!-- Mockup for Library Table -->
    <div class="w-full h-full bg-white p-4 flex flex-col">
        <div class="flex items-center justify-between mb-4 border-b border-gray-100 pb-4">
            <div class="flex items-center gap-4">
                <h3 class="font-bold text-sm">Library</h3>
                <div class="flex gap-2 text-xs text-gray-500">
                    <span class="bg-gray-100 px-2 py-1 rounded">Display: Table</span>
                    <span class="bg-gray-100 px-2 py-1 rounded">Sorted by Added</span>
                    <span class="bg-gray-100 px-2 py-1 rounded">Filter</span>
                </div>
            </div>
            <div class="w-4 h-4 bg-gray-200 rounded"></div>
        </div>
        
        <div class="w-full overflow-hidden">
            <table class="w-full text-left text-xs">
                <thead class="text-gray-400 font-medium border-b border-gray-100">
                    <tr>
                        <th class="pb-2 w-8"><input type="checkbox" class="rounded border-gray-300" /></th>
                        <th class="pb-2">Title</th>
                        <th class="pb-2">Authors</th>
                        <th class="pb-2">Added</th>
                        <th class="pb-2">Viewed</th>
                        <th class="pb-2">Tags</th>
                        <th class="pb-2">URL</th>
                    </tr>
                </thead>
                <tbody class="text-gray-600">
                    {#each [1, 2, 3, 4, 5, 6, 7] as i}
                    <tr class="border-b border-gray-50 hover:bg-gray-50">
                        <td class="py-3"><input type="checkbox" class="rounded border-gray-300" /></td>
                        <td class="py-3 font-medium text-gray-900 flex items-center gap-2">
                            <div class="w-4 h-4 bg-red-100 rounded text-[8px] flex items-center justify-center text-red-600">PDF</div>
                            DeepViT: Bridging Natural Language and Data Visu...
                        </td>
                        <td class="py-3">Shuai, et al.</td>
                        <td class="py-3">Today</td>
                        <td class="py-3">5 minutes ago</td>
                        <td class="py-3"><span class="bg-gray-100 px-1.5 py-0.5 rounded text-[10px]">attention mechani</span></td>
                        <td class="py-3 text-blue-500 underline">http://arxiv.org/a...</td>
                    </tr>
                    {/each}
                </tbody>
            </table>
        </div>
    </div>
  </FeatureScreenshot>

  <Stats />
  <Testimonials />
  <FAQ />
  <CTA />
  <Footer />
</main>

