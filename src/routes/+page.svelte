<script lang="ts">
  import Header from "$lib/components/Header.svelte";
  import Hero from "$lib/components/Hero.svelte";
  import Features from "$lib/components/Features.svelte";
  import Workflows from "$lib/components/Workflows.svelte";
  import TrustedData from "$lib/components/TrustedData.svelte";
  import AIFeatures from "$lib/components/AIFeatures.svelte";
  import Security from "$lib/components/Security.svelte";
  import Testimonial from "$lib/components/Testimonial.svelte";
  import Footer from "$lib/components/Footer.svelte";
  
  let scrollY = 0;
</script>

<svelte:window bind:scrollY />

<main class="bg-white min-h-screen font-sans selection:bg-black selection:text-white">
  <Header isScrolled={scrollY > 50} />
  <Hero />
  <Features />
  <Workflows />
  <TrustedData />
  <AIFeatures />
  <Security />
  <Testimonial />
  <Footer />
</main>

