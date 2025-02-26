<script>
  import logo_fb from '$lib/assets/logos/facebook.svg';
  import logo_ig from '$lib/assets/logos/instagram.svg';
  import logo_yt from '$lib/assets/logos/youtube_primary.svg';
  import logo_ha from '$lib/assets/logos/helloasso.svg';
  const socials = [
    { name: 'Youtube', logo: logo_yt, link: 'http://youtube.com/@amevssorbonneuniversite' },
    { name: 'Instagram', logo: logo_ig, link: 'https://www.instagram.com/amevs_su' },
    { name: 'Facebook', logo: logo_fb, link: 'http://facebook.com/AMEVS.SU' },
    { name: 'HelloAsso', logo: logo_ha, link: 'https://www.helloasso.com/associations/amevs' }
  ];
  console.log('test');
</script>

<div class="hero bg-secondary text-secondary-content lg:min-h-auto lg:p-16">HELLOOOOO</div>
<div id="socials" class="hero bg-secondary text-secondary-content lg:min-h-auto lg:p-16">
  <div class="hero-content p-6 text-center">
    <div class="max-w-md">
      <h1 class="text-5xl font-bold">Suivez Nous !</h1>
      <p class="py-6 lg:text-lg">
        Restez au courant des dernières nouvelles et des événements qui nous concernent en nous
        suivant sur les réseaux sociaux.
      </p>
      <div class="grid grid-cols-4 content-stretch items-stretch gap-4">
        <!-- {#each socials as social}
          <button class="btn btn-primary h-full w-full p-4">
            <a href={social.link} target="_blank">
              <img
                class="fill-primary-content aspect-square h-full w-full"
                src={social.logo}
                alt={social.name}
              />
            </a>
          </button>
        {/each} -->
      </div>
    </div>
  </div>
</div>
