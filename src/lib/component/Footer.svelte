<script>
  import logo_fb from '$lib/assets/logos/facebook.svg';
  import logo_ig from '$lib/assets/logos/instagram.svg';
  import logo_yt from '$lib/assets/logos/youtube_neutral.svg';
  import logo_ha from '$lib/assets/logos/helloasso.svg';
  import LogoAmevs from '$lib/assets/logos/logo_amevs.svelte';
  const socials = [
    { name: 'Youtube', logo: logo_yt, link: 'http://youtube.com/@amevssorbonneuniversite' },
    { name: 'Instagram', logo: logo_ig, link: 'https://www.instagram.com/amevs_su' },
    { name: 'Facebook', logo: logo_fb, link: 'http://facebook.com/AMEVS.SU' },
    { name: 'HelloAsso', logo: logo_ha, link: 'https://www.helloasso.com/associations/amevs' }
  ];
</script>

<footer class="footer sm:footer-horizontal bg-neutral text-neutral-content p-10">
  <aside>
    <a href="/" aria-label="Retour à la page d'accueil">
      <!-- <img src={logo_amevs} alt="Logo AMEVS" class="h-12 w-12 fill-current stroke-current" /> -->
      <LogoAmevs />
    </a>
    <p>
      AMEVS -
      <br />
      Association Musicale et Éducative à Vocation Sociale
    </p>
  </aside>
  <nav>
    <h6 class="footer-title">Social</h6>
    <div class="grid grid-flow-col gap-4">
      {#each socials as social}
        <a href={social.link} target="_blank">
          <img class="h-6 w-6" src={social.logo} alt={social.name} />
        </a>
      {/each}
    </div>
    <div class="my-5">
      <a href="mentions-legales">Mentions légales</a>
    </div>
  </nav>
</footer>
