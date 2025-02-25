<script>
  import Card from '$lib/component/Card.svelte';
</script>

<div id="project" class="bg-base-200 hero min-h-dvh">
  <div class="hero-content flex-col">
    <div class="w-full lg:mb-8 lg:flex lg:justify-between lg:self-start">
      <h1 class="text-5xl font-bold">Nos Projets</h1>
      <a class="btn-lg btn btn-primary hidden lg:inline content-center">Voir tous nos projets</a>
    </div>
    <div class="flex grow basis-0 flex-col items-center justify-center gap-4 lg:flex-row">
      <Card
        title="Concert en BU"
        description="Tout au long de l'année académique, Sorbonne Université vibre au son de concerts variés offerts aux étudiants et au personnel, transformant chaque pause midi en un moment de détente et de découverte musicale."
        img="https://img.daisyui.com/images/stock/photo-1606107557195-0e29a4b5b4aa.webp"
      />
      <Card
        title="Conférence"
        description="Notre cycle de conférences annuel explore l’histoire et l’évolution des musiques du monde, mettant à l’honneur les influences afros-diasporiques, caribéennes et haïtiennes, grâce à la collaboration de chercheurs et musiciens passionnés."
        img="https://img.daisyui.com/images/stock/photo-1606107557195-0e29a4b5b4aa.webp"
      />
      <Card
        title="Projet PAQÉMO"
        description="Fondé en 2022, PAQÉMO initie les jeunes de 6 à 18 ans à la pratique musicale tout en créant des opportunités d'emploi et en dynamisant la scène musicale haïtienne, pour un impact culturel et social durable."
        img="https://img.daisyui.com/images/stock/photo-1606107557195-0e29a4b5b4aa.webp"
      />
    </div>
    <a class="btn-lg btn btn-primary lg:hidden">Voir tous nos projets</a>
  </div>
</div>
