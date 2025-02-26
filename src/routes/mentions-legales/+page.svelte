<script>
  import Footer from '$lib/component/Footer.svelte';
  import HeaderSubPage from '$lib/component/HeaderSubPage.svelte';
</script>

<HeaderSubPage />
<div class="flex min-h-dvh flex-col gap-4 p-16 bg-base-200">
	<h1 class="text-5xl">Mentions légales</h1>
  <div>
    <p>
      Le site amevs.fr est la propriété de l'Association Musicale et Éducative à Vocation Sociale
      loi 1901 à but non lucratif reconnue publique au JO du XX/XX/XX, dont le siège social est
      situé au 4 Place Jussieu 75005 Paris.<br />
      SIRET XXXXXXX <br />
      Tél. : +33 (0)7 55 90 57 02 <br />
      Courriel : amevs.su@gmail.com
    </p>
  </div>
  <div>
    <h2 class="text-2xl">Réalisation et maintenance technique</h2>
    <p>
      Le site amevs.fr est réalisé par <a href="https://charles.vin/" class="link">Charles Vin</a>.
    </p>
  </div>
  <div>
    <h2 class="text-2xl">Hébergement</h2>
    <p>
      Le site amevs.fr est hébergé par <a href="cloudflare.com" class="link">Cloudflare</a>, Inc.
      101 Townsend St, San Francisco, CA 94107 USA
    </p>
  </div>
</div>
<Footer />
