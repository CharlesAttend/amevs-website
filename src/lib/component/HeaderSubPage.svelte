<script>
  import LogoAmevs from "$lib/assets/logos/logo_amevs.svelte";

  let breadCrumb = [
    { title: 'Accueil', link: '/' },
    { title: 'Mentions légales', link: '/mentions-legales' }
  ];
</script>

<header class="w-full bg-white">
  <nav class="mx-auto flex max-w-7xl items-center justify-between p-6 lg:px-8" aria-label="Global">
    <div class="flex">
      <a href="/" class="p-1.5">
        <span class="sr-only">AMEVS</span>
        <LogoAmevs classAttributes="fill-current w-8"/>
      </a>
    </div>
    <div class="breadcrumbs text-sm s">
      <ul>
        {#each breadCrumb as item}
          <li><a href={item.link}>{item.title}</a></li>
        {/each}
      </ul>
    </div>
  </nav>
</header>
