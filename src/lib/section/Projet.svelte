<script>
  import Card from '$lib/component/Card.svelte';
</script>

<div id="project" class="bg-base-200 hero min-h-screen">
  <div class="hero-content flex-col lg:flex-row">
    <div>
      <h1 class="text-5xl font-bold">Nos Projets</h1>
      <!-- <button>Vois tous nos projets</button> -->
    </div>
    <div class="flex flex-col items-center justify-center gap-4">
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
  </div>
  <!-- <button>Vois tous nos projets</button> -->
</div>
