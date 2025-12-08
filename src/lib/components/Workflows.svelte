<script>
  const workflowItems = [
    {
      title: 'Smart Episode Discovery',
      description: 'Our AI analyzes your interests and listening patterns to surface the most relevant episodes from our curated network. Never miss insights that matter to your role and industry.',
      type: 'workflow'
    },
    {
      title: 'Instant AI Summaries',
      description: 'Every episode comes with an AI-generated report highlighting key insights, actionable takeaways, and relevant timestamps. Get the value in minutes, not hours.',
      type: 'table'
    },
    {
      title: 'Community Insights',
      description: 'Connect with fellow marketing leaders, share perspectives, and discover what your peers are learning. Transform passive listening into active knowledge sharing.',
      type: 'creation'
    }
  ];
</script>

<section class="py-24 bg-white">
  <div class="max-w-[1400px] mx-auto px-6">
    <div class="mb-16">
      <h2 class="text-4xl md:text-5xl font-serif text-gray-900 mb-4">From Passive Listening<br/>to Active Intelligence</h2>
    </div>

    <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
      {#each workflowItems as item}
        <div class="group">
          <!-- Card Visual -->
          <div class="bg-primary-900 rounded-lg overflow-hidden aspect-[4/3] mb-8 relative p-6 flex flex-col">
            {#if item.type === 'workflow'}
               <!-- Workflow UI Mockup -->
               <div class="bg-white rounded-md shadow-lg p-4 w-full h-full flex flex-col gap-3 text-[10px]">
                  <div class="flex items-center gap-2 border-b pb-2">
                     <div class="w-4 h-4 bg-primary-100 rounded flex items-center justify-center text-primary-700">✓</div>
                     <span class="font-medium">Discovering Episodes for You</span>
                  </div>
                  <div class="space-y-2 pl-2">
                     <div class="flex items-center gap-2">
                        <div class="w-3 h-3 bg-primary-500 rounded-full animate-pulse"></div>
                        <span class="font-medium">Analyzing preferences...</span>
                     </div>
                     <div class="flex items-center gap-2 text-gray-500">
                        <div class="w-3 h-3 border border-gray-300 rounded-full flex items-center justify-center text-[8px]">✓</div>
                        <span>Reviewing listening history</span>
                     </div>
                     <div class="flex items-center gap-2 text-gray-500">
                        <div class="w-3 h-3 border border-gray-300 rounded-full flex items-center justify-center text-[8px]">✓</div>
                        <span>Matching industry topics</span>
                     </div>
                     <div class="flex items-center gap-2 text-gray-500">
                        <div class="w-3 h-3 border border-gray-300 rounded-full flex items-center justify-center text-[8px]">✓</div>
                        <span>Filtering by relevance</span>
                     </div>
                     <div class="flex items-center gap-2 text-gray-500">
                        <div class="w-3 h-3 border border-gray-300 rounded-full flex items-center justify-center text-[8px]">✓</div>
                        <span>Curating recommendations</span>
                     </div>
                     <div class="flex items-center gap-2 text-gray-500">
                        <div class="w-3 h-3 border border-gray-300 rounded-full flex items-center justify-center text-[8px]"></div>
                        <span>Preparing queue...</span>
                     </div>
                  </div>
               </div>
            {:else if item.type === 'table'}
               <!-- Table UI Mockup -->
               <div class="bg-white rounded-md shadow-lg p-4 w-full h-full flex flex-col gap-2 text-[10px]">
                  <div class="flex justify-between items-center mb-1">
                     <span class="font-medium text-gray-700">Tariff impact on top manufacturing firms</span>
                  </div>
                  <div class="flex items-center gap-2 text-gray-500 mb-2">
                     <div class="w-4 h-4 bg-gray-100 rounded flex items-center justify-center">🔍</div>
                     <span>Found 12 sources</span>
                  </div>
                  <p class="text-gray-400 text-[9px] mb-3">Currently, Caterpillar, Boeing, and Ford face tariff pressures among leading U.S. manufacturers.</p>
                  
                  <div class="border rounded overflow-hidden">
                     <div class="grid grid-cols-2 bg-gray-50 p-1.5 border-b font-medium text-gray-600">
                        <div>Company</div>
                        <div>% Revenue from Int.</div>
                     </div>
                     <div class="grid grid-cols-2 p-1.5 border-b items-center">
                        <div class="flex items-center gap-1"><div class="w-2 h-2 border rounded-sm"></div> General Electric</div>
                        <div class="h-1.5 bg-gray-200 rounded w-16"></div>
                     </div>
                     <div class="grid grid-cols-2 p-1.5 border-b items-center">
                        <div class="flex items-center gap-1"><div class="w-2 h-2 border rounded-sm"></div> Boeing</div>
                        <div class="h-1.5 bg-gray-200 rounded w-12"></div>
                     </div>
                     <div class="grid grid-cols-2 p-1.5 items-center">
                        <div class="flex items-center gap-1"><div class="w-2 h-2 border rounded-sm"></div> Caterpillar</div>
                        <div class="h-1.5 bg-gray-200 rounded w-14"></div>
                     </div>
                  </div>
               </div>
            {:else}
               <!-- Creation UI Mockup -->
               <div class="bg-white rounded-md shadow-lg p-4 w-full h-full flex flex-col gap-3 text-[10px]">
                  <div class="flex items-center gap-2 mb-2">
                     <div class="w-4 h-4 bg-primary-600 rounded flex items-center justify-center text-white text-[8px]">
                        <svg xmlns="http://www.w3.org/2000/svg" width="10" height="10" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M17 18a2 2 0 0 0-2-2H9a2 2 0 0 0-2 2"/><rect width="18" height="18" x="3" y="4" rx="2"/><circle cx="12" cy="10" r="2"/><line x1="8" x2="8" y1="2" y2="4"/><line x1="16" x2="16" y1="2" y2="4"/></svg>
                     </div>
                     <span class="text-gray-500">Community discussion</span>
                  </div>
                  <div class="bg-gray-50 p-3 rounded border border-gray-100">
                     <p class="text-gray-600 mb-3 text-[9px]">Sarah Chen shared insights from "The Future of Brand Communities"</p>
                     <div class="text-[9px] text-gray-400 mb-2">3 comments</div>
                     <div class="space-y-2">
                        <div class="bg-white p-2 rounded border border-gray-200">
                           <div class="flex items-center gap-2 mb-1">
                              <div class="w-3 h-3 bg-gray-300 rounded-full"></div>
                              <span class="font-medium text-[9px]">Mike R.</span>
                           </div>
                           <p class="text-[8px] text-gray-500">We're testing this approach...</p>
                        </div>
                        <div class="bg-white p-2 rounded border border-gray-200">
                           <div class="flex items-center gap-2 mb-1">
                              <div class="w-3 h-3 bg-gray-300 rounded-full"></div>
                              <span class="font-medium text-[9px]">Lisa K.</span>
                           </div>
                           <p class="text-[8px] text-gray-500">Great episode! The ROI data...</p>
                        </div>
                     </div>
                  </div>
               </div>
            {/if}
          </div>
          
          <h3 class="text-xl font-serif text-gray-900 mb-3">{item.title}</h3>
          <p class="text-sm leading-relaxed text-gray-500 font-light">{item.description}</p>
        </div>
      {/each}
    </div>
  </div>
</section>
