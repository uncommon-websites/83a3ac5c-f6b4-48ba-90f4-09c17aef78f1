<script>
  const providers = [
    { name: "Your Firm's Data", icon: "database" },
    { name: "LSEG", icon: "globe" },
    { name: "Dow Jones", icon: "activity" },
    { name: "FactSet", icon: "bar-chart" },
    { name: "Capital IQ", icon: "pie-chart" },
    { name: "PitchBook", icon: "book" },
    { name: "Preqin", icon: "search" },
    { name: "Real-time Web & News", icon: "globe" },
    { name: "SEC Filings", icon: "file-text" },
    { name: "Transcripts", icon: "mic" },
    { name: "Investor Presentations", icon: "monitor" },
    { name: "International Filings", icon: "file" }
  ];
</script>

<section class="py-24 bg-white">
  <div class="max-w-[1400px] mx-auto px-6">
    <div class="mb-16">
      <h2 class="text-4xl md:text-5xl font-serif text-gray-900 mb-6">Curated Network</h2>
      <p class="text-gray-500 max-w-2xl font-light text-lg">
        We partner with leading voices in marketing and business to bring you the highest-quality podcast content. Our curated network, combined with AI-powered insights, gives you the clarity and confidence to stay ahead of industry trends.
      </p>
    </div>

    <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-4">
      {#each providers as provider}
        <div class="flex items-center gap-4 p-6 bg-gray-50 rounded-lg hover:bg-gray-100 transition-colors cursor-default">
          <div class="w-10 h-10 bg-white rounded shadow-sm flex items-center justify-center text-gray-700">
             <!-- Placeholder Icon -->
             <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round">
                {#if provider.icon === 'database'}
                  <ellipse cx="12" cy="5" rx="9" ry="3"/><path d="M21 12c0 1.66-4 3-9 3s-9-1.34-9-3"/><path d="M3 5v14c0 1.66 4 3 9 3s9-1.34 9-3V5"/>
                {:else if provider.icon === 'globe'}
                  <circle cx="12" cy="12" r="10"/><line x1="2" x2="22" y1="12" y2="12"/><path d="M12 2a15.3 15.3 0 0 1 4 10 15.3 15.3 0 0 1-4 10 15.3 15.3 0 0 1-4-10 15.3 15.3 0 0 1 4-10z"/>
                {:else if provider.icon === 'activity'}
                  <polyline points="22 12 18 12 15 21 9 3 6 12 2 12"/>
                {:else if provider.icon === 'bar-chart'}
                  <line x1="12" x2="12" y1="20" y2="10"/><line x1="18" x2="18" y1="20" y2="4"/><line x1="6" x2="6" y1="20" y2="16"/>
                {:else if provider.icon === 'pie-chart'}
                  <path d="M21.21 15.89A10 10 0 1 1 8 2.83"/><path d="M22 12A10 10 0 0 0 12 2v10z"/>
                {:else if provider.icon === 'book'}
                  <path d="M4 19.5A2.5 2.5 0 0 1 6.5 17H20"/><path d="M6.5 2H20v20H6.5A2.5 2.5 0 0 1 4 19.5v-15A2.5 2.5 0 0 1 6.5 2z"/>
                {:else if provider.icon === 'search'}
                  <circle cx="11" cy="11" r="8"/><line x1="21" x2="16.65" y1="21" y2="16.65"/>
                {:else if provider.icon === 'file-text'}
                  <path d="M14.5 2H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V7.5L14.5 2z"/><polyline points="14 2 14 8 20 8"/><line x1="16" x2="8" y1="13" y2="13"/><line x1="16" x2="8" y1="17" y2="17"/><line x1="10" x2="8" y1="9" y2="9"/>
                {:else if provider.icon === 'mic'}
                  <path d="M12 1a3 3 0 0 0-3 3v8a3 3 0 0 0 6 0V4a3 3 0 0 0-3-3z"/><path d="M19 10v2a7 7 0 0 1-14 0v-2"/><line x1="12" x2="12" y1="19" y2="23"/><line x1="8" x2="16" y1="23" y2="23"/>
                {:else if provider.icon === 'monitor'}
                  <rect height="14" rx="2" ry="2" width="20" x="2" y="3"/><line x1="8" x2="16" y1="21" y2="21"/><line x1="12" x2="12" y1="17" y2="21"/>
                {:else}
                  <path d="M14 2H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V8z"/><polyline points="14 2 14 8 20 8"/><line x1="16" x2="8" y1="13" y2="13"/><line x1="16" x2="8" y1="17" y2="17"/><polyline points="10 9 9 9 8 9"/>
                {/if}
             </svg>
          </div>
          <span class="text-gray-900 font-serif text-lg">{provider.name}</span>
        </div>
      {/each}
    </div>
  </div>
</section>
