<script>
  import { setGlobalOptions } from 'svelte-scrolling';
  setGlobalOptions({
    offset: -75,
    passive: true
  });

  import Header from '$lib/component/Header.svelte';
  import Hero from '$lib/section/Hero.svelte';
  import SocialProof from '$lib/section/SocialProof.svelte';
  import Footer from '$lib/component/Footer.svelte';
  import Presentation from '$lib/section/Presentation.svelte';
  import Vision from '$lib/section/Vision.svelte';
  import Projet from '$lib/section/Projet.svelte';
  import Statistiques from '$lib/section/Statistiques.svelte';
  import Temoignage from '$lib/section/Temoignage.svelte';
  import Membre from '$lib/section/Membre.svelte';
  import Socials from '$lib/section/Socials.svelte';
</script>

<div class="overflow-x-hidden">
  <Header />
  <Hero />
  <SocialProof />
  <Presentation />
  <Vision />
  <Projet />
  <Statistiques />
  <Temoignage />
  <Membre />
  <Socials />
  <Footer />
</div>
