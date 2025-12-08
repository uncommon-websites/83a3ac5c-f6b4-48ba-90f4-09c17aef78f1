<script>
</script>

<section class="py-24 bg-[#111111] text-white">
  <div class="max-w-[1400px] mx-auto px-6">
    <div class="grid grid-cols-1 lg:grid-cols-2 gap-16">
      <div class="flex flex-col justify-between">
        <div>
          <div class="flex items-center gap-2 mb-16">
            <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><rect width="18" height="11" x="3" y="11" rx="2" ry="2"/><path d="M7 11V7a5 5 0 0 1 10 0v4"/></svg>
            <span class="text-sm font-medium tracking-wider uppercase">Security</span>
          </div>

          <h2 class="text-4xl md:text-5xl font-serif mb-8">
            Built for Enterprise<br/>Secure by Design
          </h2>

          <div class="space-y-4 mb-12">
            <div class="flex items-center gap-3 text-gray-400">
              <svg xmlns="http://www.w3.org/2000/svg" width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><rect width="18" height="11" x="3" y="11" rx="2" ry="2"/><path d="M7 11V7a5 5 0 0 1 10 0v4"/></svg>
              <span>No training on your data</span>
            </div>
            <div class="flex items-center gap-3 text-gray-400">
              <svg xmlns="http://www.w3.org/2000/svg" width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M17.5 19c0-1.7-1.3-3-3-3h-5c-1.7 0-3 1.3-3 3"/><path d="M22 19a2 2 0 0 0-2-2h-2a2 2 0 0 0-2 2"/><path d="M12 16a2 2 0 0 1 2-2h2a2 2 0 0 1 2 2"/><path d="M8 16a2 2 0 0 0-2-2H4a2 2 0 0 0-2 2"/><path d="M12 12a3 3 0 1 0 0-6 3 3 0 0 0 0 6Z"/></svg>
              <span>Modern & secure data practices</span>
            </div>
            <div class="flex items-center gap-3 text-gray-400">
              <svg xmlns="http://www.w3.org/2000/svg" width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M12 22s8-4 8-10V5l-8-3-8 3v7c0 6 8 10 8 10z"/></svg>
              <span>End to end encryption</span>
            </div>
            <div class="flex items-center gap-3 text-gray-400">
              <svg xmlns="http://www.w3.org/2000/svg" width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><polyline points="16 18 22 12 16 6"/><polyline points="8 6 2 12 8 18"/></svg>
              <span>Audited & tested</span>
            </div>
          </div>
        </div>

        <a href="#privacy" class="inline-flex items-center gap-2 text-sm text-gray-400 hover:text-white transition-colors group">
          Read our privacy policy
          <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="group-hover:translate-x-1 transition-transform"><line x1="5" y1="12" x2="19" y2="12"/><polyline points="12 5 19 12 12 19"/></svg>
        </a>
      </div>

      <div class="grid grid-cols-2 gap-px bg-gray-800 border border-gray-800">
        <div class="bg-[#111111] aspect-square flex flex-col items-center justify-center p-8 text-center group hover:bg-[#161616] transition-colors">
          <div class="w-20 h-20 rounded-full border border-gray-700 flex items-center justify-center mb-4 group-hover:border-gray-500 transition-colors">
             <span class="font-serif text-xs text-gray-400">AICPA</span>
             <span class="font-bold text-xs ml-1">SOC 2</span>
          </div>
          <span class="text-xs text-gray-500 uppercase tracking-widest">SOC2</span>
        </div>
        <div class="bg-[#111111] aspect-square flex flex-col items-center justify-center p-8 text-center group hover:bg-[#161616] transition-colors">
          <div class="w-20 h-20 flex items-center justify-center mb-4">
             <!-- California Map Approximation -->
             <svg viewBox="0 0 100 100" fill="currentColor" class="w-16 h-16 text-gray-700 group-hover:text-gray-500 transition-colors">
                <path d="M25,10 L45,10 L80,35 L65,90 L35,85 L15,40 Z" /> 
             </svg>
          </div>
          <span class="text-xs text-gray-500 uppercase tracking-widest">CCPA</span>
        </div>
        <div class="bg-[#111111] aspect-square flex flex-col items-center justify-center p-8 text-center group hover:bg-[#161616] transition-colors">
          <div class="w-20 h-20 rounded-full border border-gray-700 flex items-center justify-center mb-4 group-hover:border-gray-500 transition-colors">
             <div class="text-center">
                <div class="text-[10px] font-bold text-gray-400">ISO</div>
                <div class="text-[8px] text-gray-400">27001</div>
             </div>
             <div class="absolute inset-0 rounded-full border border-gray-800 scale-110"></div>
             <div class="absolute inset-0 rounded-full border border-gray-800 scale-125"></div>
          </div>
          <span class="text-xs text-gray-500 uppercase tracking-widest">ISO 27001</span>
        </div>
        <div class="bg-[#111111] aspect-square flex flex-col items-center justify-center p-8 text-center group hover:bg-[#161616] transition-colors">
          <div class="w-20 h-20 flex items-center justify-center mb-4 relative">
             {#each Array(12) as _, i}
                <div class="absolute w-1 h-1 bg-gray-600 rounded-full" style="transform: rotate({i * 30}deg) translate(24px)"></div>
             {/each}
             <div class="text-[8px] font-bold text-gray-600">EU</div>
          </div>
          <span class="text-xs text-gray-500 uppercase tracking-widest">GDPR</span>
        </div>
      </div>
    </div>
  </div>
</section>
