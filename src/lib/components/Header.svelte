<script>
  export let isScrolled = false;
</script>

<header class="fixed top-0 left-0 w-full z-50 transition-all duration-300 {isScrolled ? 'bg-white/90 backdrop-blur-md py-4 shadow-sm' : 'bg-transparent py-6'}">
  <div class="max-w-[1400px] mx-auto px-6 flex items-center justify-between">
    <!-- Logo -->
    <a href="/" class="text-2xl font-medium tracking-tight font-sans">rogo</a>

    <!-- Nav -->
    <nav class="hidden md:flex items-center gap-8">
      <a href="#product" class="text-sm font-medium text-gray-600 hover:text-black transition-colors">Product</a>
      <a href="#security" class="text-sm font-medium text-gray-600 hover:text-black transition-colors">Security</a>
      <a href="#company" class="text-sm font-medium text-gray-600 hover:text-black transition-colors">Company</a>
      <a href="#news" class="text-sm font-medium text-gray-600 hover:text-black transition-colors">News</a>
      <a href="#careers" class="text-sm font-medium text-gray-600 hover:text-black transition-colors">Careers</a>
    </nav>

    <!-- Actions -->
    <div class="flex items-center gap-6">
      <a href="#login" class="text-sm font-medium text-gray-600 hover:text-black transition-colors">Log in</a>
      <a href="#demo" class="bg-black text-white text-sm font-medium px-5 py-2.5 rounded-full hover:bg-gray-800 transition-colors">
        Request Demo
      </a>
    </div>
  </div>
</header>
