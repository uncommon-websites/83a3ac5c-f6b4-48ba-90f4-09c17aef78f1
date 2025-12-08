<script>
  const features = [
    {
      id: '01',
      title: 'AI-powered episode insights',
      active: true
    },
    {
      id: '02',
      title: 'Curated for marketing leaders',
      active: false
    },
    {
      id: '03',
      title: 'Community of the curious',
      active: false
    },
    {
      id: '04',
      title: 'Actionable, not passive',
      active: false
    }
  ];
</script>

<section class="py-24 max-w-[1400px] mx-auto px-6">
  <div class="mb-20">
    <h2 class="text-4xl md:text-5xl font-serif text-gray-900 leading-tight max-w-4xl">
      Marketing media is fragmented and overwhelming. <span class="font-semibold">Bubbler delivers the signal through the noise.</span>
    </h2>
  </div>

  <div class="grid grid-cols-1 lg:grid-cols-2 gap-16 items-start">
    <!-- Left: Image/UI Preview -->
    <div class="relative bg-primary-900 rounded-lg overflow-hidden aspect-[4/3] shadow-2xl">
      <img 
        src="/generated/image-marketing-professionals-collaborating-in-1765148114641-1.webp" 
        alt="Marketing professionals collaborating" 
        class="absolute inset-0 w-full h-full object-cover opacity-30 mix-blend-overlay"
      />
      
      <!-- UI Overlay -->
      <div class="absolute inset-0 flex items-center justify-center p-8">
        <div class="bg-white/95 backdrop-blur rounded-lg shadow-lg w-full max-w-md p-6">
           <div class="flex items-center gap-4 mb-4">
              <div class="w-12 h-12 bg-primary-600 rounded-lg flex items-center justify-center text-white">
                <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M12 2a3 3 0 0 0-3 3v7a3 3 0 0 0 6 0V5a3 3 0 0 0-3-3Z"/><path d="M19 10v2a7 7 0 0 1-14 0v-2"/><line x1="12" x2="12" y1="19" y2="22"/></svg>
              </div>
              <div class="flex-1">
                 <div class="text-xs text-gray-400 mb-1">Latest Episode</div>
                 <div class="text-sm font-semibold text-gray-900">
                    The Future of Brand Communities
                 </div>
                 <div class="text-xs text-gray-500 mt-1">Marketing Mindset • 28 min</div>
              </div>
           </div>
           <div class="h-px bg-gray-100 w-full my-3"></div>
           <div class="bg-secondary-50 p-3 rounded text-xs text-gray-700">
              <strong class="text-secondary-900">AI Summary:</strong> Brand communities drive 2.4x higher customer lifetime value. Focus on authentic connections over transactions...
           </div>
        </div>
      </div>
    </div>

    <!-- Right: Features List -->
    <div class="pt-8">
      <h3 class="text-3xl font-serif text-gray-900 mb-12">
        A Community of Curious<br/>Marketing Leaders
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
