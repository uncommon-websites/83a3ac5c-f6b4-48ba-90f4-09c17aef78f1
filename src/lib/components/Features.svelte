<script>
  const features = [
    {
      id: '01',
      title: 'All your content in one place',
      active: true
    },
    {
      id: '02',
      title: 'Transparent, auditable sources',
      active: false
    },
    {
      id: '03',
      title: 'Automate your workflows',
      active: false
    },
    {
      id: '04',
      title: 'Proprietary document interrogation',
      active: false
    }
  ];
</script>

<section class="py-24 max-w-[1400px] mx-auto px-6">
  <div class="mb-20">
    <h2 class="text-4xl md:text-5xl font-serif text-gray-900 leading-tight max-w-4xl">
      Just as Bloomberg digitized financial data in the 1980s, <span class="font-semibold">Rogo is now transforming financial workflows.</span>
    </h2>
  </div>

  <div class="grid grid-cols-1 lg:grid-cols-2 gap-16 items-start">
    <!-- Left: Image/UI Preview -->
    <div class="relative bg-gray-900 rounded-lg overflow-hidden aspect-[4/3] shadow-2xl">
      <img 
        src="https://images.unsplash.com/photo-1486406146926-c627a92ad1ab?q=80&w=2070&auto=format&fit=crop" 
        alt="Financial Data" 
        class="absolute inset-0 w-full h-full object-cover opacity-40 mix-blend-overlay"
      />
      
      <!-- UI Overlay -->
      <div class="absolute inset-0 flex items-center justify-center p-8">
        <div class="bg-white/95 backdrop-blur rounded-lg shadow-lg w-full max-w-md p-6">
           <div class="flex items-center gap-4 mb-4">
              <button class="p-2 hover:bg-gray-100 rounded-full">
                <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="m15 18-6-6 6-6"/></svg>
              </button>
              <div class="flex-1">
                 <div class="text-xs text-gray-400 mb-1">Filings and earnings</div>
                 <div class="flex items-center gap-2 text-sm font-medium">
                    <div class="w-5 h-5 bg-blue-600 rounded flex items-center justify-center text-white text-[10px]">
                      <svg xmlns="http://www.w3.org/2000/svg" width="12" height="12" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M3 3v18h18"/><path d="m19 9-5 5-4-4-3 3"/></svg>
                    </div>
                    Market data
                 </div>
              </div>
           </div>
           <div class="h-px bg-gray-100 w-full my-2"></div>
           <div class="pl-12 text-sm text-gray-400">Investor presentations</div>
        </div>
      </div>
    </div>

    <!-- Right: Features List -->
    <div class="pt-8">
      <h3 class="text-3xl font-serif text-gray-900 mb-12">
        An Integrated, Secure Platform<br/>Built to Drive Your Firm Forward
      </h3>

      <div class="space-y-8">
        {#each features as feature}
          <div class="flex items-center gap-6 group cursor-pointer">
            <div class="relative w-12 h-12 flex items-center justify-center">
              <!-- Circle border -->
              <div class="absolute inset-0 border-2 rounded-full transition-colors duration-300 {feature.active ? 'border-black' : 'border-gray-200 group-hover:border-gray-300'}"></div>
              
              <!-- Brackets for active state -->
              {#if feature.active}
                <div class="absolute -left-1 top-1/2 -translate-y-1/2 w-2 h-4 bg-white"></div>
                <div class="absolute -right-1 top-1/2 -translate-y-1/2 w-2 h-4 bg-white"></div>
                <div class="absolute inset-0 flex items-center justify-center">
                   <div class="absolute left-0 top-1/2 -translate-y-1/2 -translate-x-1/2 font-serif text-2xl font-light">[</div>
                   <div class="absolute right-0 top-1/2 -translate-y-1/2 translate-x-1/2 font-serif text-2xl font-light">]</div>
                </div>
              {/if}

              <span class="text-sm font-medium {feature.active ? 'text-black' : 'text-gray-400'}">{feature.id}</span>
            </div>
            <span class="text-lg {feature.active ? 'text-gray-900 font-medium' : 'text-gray-500 font-light'}">{feature.title}</span>
          </div>
        {/each}
      </div>
    </div>
  </div>
</section>
