<script>
  import logo_su from '$lib/assets/Logo_of_Sorbonne_University.svg';
  import logo_inst2france from '$lib/assets/Institut_de_France_logo.svg';
  import logo_orchestre_ecole from '$lib/assets/logo-oae_RVB.svg';
</script>

<div class="hero bg-base-100 min-h-screen">
  <div class="hero-content text-center">
    <div class="max-w-md">
      <h1 class="text-5xl font-bold">Nos partenaires</h1>
      <!-- <p class="py-6">167 instrument de musique donnés</p> -->
      <div class="flex flex-wrap justify-center gap-1 py-6">
        <img src={logo_su} alt="Sorbonne University" class="max-w-1/2" />
        <img src={logo_orchestre_ecole} alt="Orchestre à l'école" class="max-w-1/2" />
        <img src={logo_inst2france} alt="Institut de France" class="max-w-1/2" />
      </div>
      <button class="btn btn-primary">Donner un instrument</button>
    </div>
  </div>
</div>
