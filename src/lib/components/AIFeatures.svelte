<script>
  const features = [
    {
      title: 'Integrations',
      description: 'Connect seamlessly with your existing providers and file systems. Enhance your workflows by interacting with internal & external data sources.',
      type: 'integrations'
    },
    {
      title: 'Prompt Library',
      description: 'Choose from our library of professionally written prompts aimed at automating your common workflows end-to-end.',
      type: 'library'
    },
    {
      title: 'Guided Implementation',
      description: 'White-glove engagement and implementation with our team of ex-bankers and private equity investors.',
      type: 'implementation'
    },
    {
      title: 'Custom-Trained Models',
      description: 'Custom-trained LLMs built for finance, using professionally labeled data tailored to the workflows and precision standards of investment banking.',
      type: 'models'
    },
    {
      title: 'Governance & Permissions',
      description: 'Granular permission controls, role-based access management, comprehensive audit trails, and customizable governance policies to streamline compliance and safeguard your data.',
      type: 'governance'
    },
    {
      title: 'Single Tenant Deployment',
      description: 'Flexible deployment options to meet your security and infrastructure needs.',
      type: 'deployment'
    }
  ];
</script>

<section class="py-24 bg-white">
  <div class="max-w-[1400px] mx-auto px-6">
    <div class="mb-16">
      <h2 class="text-4xl md:text-5xl font-serif text-gray-900 leading-tight">
        Intelligence That Adapts<br/>to Your Marketing Goals
      </h2>
    </div>

    <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
      {#each features as feature}
        <div class="bg-gray-50 p-8 rounded-lg flex flex-col h-full">
          <h3 class="text-xl font-serif text-gray-900 mb-8">{feature.title}</h3>
          
          <div class="flex-1 flex items-center justify-center mb-8 min-h-[160px]">
             {#if feature.type === 'integrations'}
                <div class="grid grid-cols-2 gap-4">
                   <div class="w-10 h-10 bg-white shadow rounded flex items-center justify-center text-gray-400">
                      <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><ellipse cx="12" cy="5" rx="9" ry="3"/><path d="M21 12c0 1.66-4 3-9 3s-9-1.34-9-3"/><path d="M3 5v14c0 1.66 4 3 9 3s9-1.34 9-3V5"/></svg>
                   </div>
                   <div class="w-10 h-10 bg-white shadow rounded flex items-center justify-center text-blue-600">
                      <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M14.5 2H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V7.5L14.5 2z"/><polyline points="14 2 14 8 20 8"/></svg>
                   </div>
                   <div class="w-10 h-10 bg-white shadow rounded flex items-center justify-center text-orange-500">
                      <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M4 22h14a2 2 0 0 0 2-2V7.5L14.5 2H6a2 2 0 0 0-2 2v4"/><path d="M14 2v6h6"/><path d="m3 15 2.5 2.5L8 15"/></svg>
                   </div>
                   <div class="w-10 h-10 bg-white shadow rounded flex items-center justify-center text-green-600">
                      <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><rect width="18" height="18" x="3" y="3" rx="2" ry="2"/><line x1="3" x2="21" y1="9" y2="9"/><line x1="9" x2="9" y1="21" y2="9"/></svg>
                   </div>
                </div>
             {:else if feature.type === 'library'}
                <div class="bg-white shadow rounded p-4 w-full max-w-[200px] text-[10px] space-y-2">
                   <div class="flex items-center gap-2 text-gray-500"><div class="w-2 h-2 rounded-full bg-gray-300"></div> Earnings Call Analysis</div>
                   <div class="flex items-center gap-2 text-gray-500"><div class="w-2 h-2 rounded-full bg-gray-300"></div> Public Company Strip Profile</div>
                   <div class="flex items-center gap-2 text-gray-500"><div class="w-2 h-2 rounded-full bg-gray-300"></div> Meeting Prep</div>
                   <div class="flex items-center gap-2 text-gray-500"><div class="w-2 h-2 rounded-full bg-gray-300"></div> Private Company Profile</div>
                   <div class="flex items-center gap-2 text-gray-500"><div class="w-2 h-2 rounded-full bg-gray-300"></div> Personal Bio</div>
                </div>
             {:else if feature.type === 'implementation'}
                <div class="flex items-center -space-x-4">
                   <div class="w-12 h-12 rounded-full border-2 border-white bg-gray-200 overflow-hidden">
                      <img src="https://images.unsplash.com/photo-1534528741775-53994a69daeb?q=80&w=200&auto=format&fit=crop" alt="User" class="w-full h-full object-cover" />
                   </div>
                   <div class="w-12 h-12 rounded-full border-2 border-white bg-gray-200 overflow-hidden z-10">
                      <img src="https://images.unsplash.com/photo-1506794778202-cad84cf45f1d?q=80&w=200&auto=format&fit=crop" alt="User" class="w-full h-full object-cover" />
                   </div>
                   <div class="w-12 h-12 rounded-full border-2 border-white bg-gray-200 overflow-hidden">
                      <img src="https://images.unsplash.com/photo-1494790108377-be9c29b29330?q=80&w=200&auto=format&fit=crop" alt="User" class="w-full h-full object-cover" />
                   </div>
                </div>
             {:else if feature.type === 'models'}
                <div class="relative w-full h-full flex items-center justify-center">
                   <div class="grid grid-cols-4 gap-2 opacity-30">
                      {#each Array(12) as _, i}
                         <div class="w-8 h-8 border border-gray-400 rounded-sm"></div>
                      {/each}
                   </div>
                   <div class="absolute inset-0 flex items-center justify-center">
                      <div class="w-10 h-10 bg-[#152e26] rounded flex items-center justify-center text-white shadow-lg">
                         <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M12 2v4"/><path d="m16.2 7.8 2.9-2.9"/><path d="M18 12h4"/><path d="m16.2 16.2 2.9 2.9"/><path d="M12 18v4"/><path d="m7.8 16.2-2.9 2.9"/><path d="M2 12h4"/><path d="m7.8 7.8-2.9-2.9"/><circle cx="12" cy="12" r="3"/></svg>
                      </div>
                   </div>
                </div>
             {:else if feature.type === 'governance'}
                <div class="bg-white shadow rounded p-4 w-full max-w-[200px] text-[10px]">
                   <div class="flex justify-between items-center mb-3">
                      <div class="font-medium">Active Users</div>
                      <div class="text-green-600">122 +8</div>
                   </div>
                   <div class="space-y-2">
                      <div class="h-1.5 bg-gray-100 rounded w-full overflow-hidden">
                         <div class="h-full bg-gray-800 w-3/4"></div>
                      </div>
                      <div class="h-1.5 bg-gray-100 rounded w-full overflow-hidden">
                         <div class="h-full bg-gray-600 w-1/2"></div>
                      </div>
                      <div class="h-1.5 bg-gray-100 rounded w-full overflow-hidden">
                         <div class="h-full bg-gray-400 w-1/4"></div>
                      </div>
                   </div>
                </div>
             {:else}
                <div class="relative">
                   <div class="w-12 h-12 bg-[#152e26] rounded flex items-center justify-center text-white relative z-10">
                      <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><rect width="18" height="18" x="3" y="3" rx="2"/><path d="M9 3v18"/><path d="m14 9 3 3-3 3"/></svg>
                   </div>
                   <div class="absolute inset-0 border border-dashed border-gray-300 rounded scale-150"></div>
                </div>
             {/if}
          </div>

          <p class="text-sm leading-relaxed text-gray-500 font-light">{feature.description}</p>
        </div>
      {/each}
    </div>
  </div>
</section>
