<script>
  import img from '$lib/assets/illustrations/vision.jpg';
</script>

<div class="hero min-h-dvh bg-secondary text-secondary-content lg:min-h-auto lg:p-16">
  <div class="hero-content flex-col lg:flex-row lg:max-w-auto lg:item-stretch">
    <img
      src={img}
      alt="Jeune fille souriante jouant du violon"
      class="max-w-sm w-full rounded-full shadow-2xl lg:w-1/2 lg:max-w-auto"
    />
    <div class="flex flex-col items-start justify-start gap-6 lg:p-20 lg:w-1/2">
      <h1 class="text-5xl font-bold">Notre vision</h1>
      <p class="">
        Être un acteur clé du rayonnement mondial de la culture, offrant aux jeunes une vie
        épanouissante, en particulier à ceux des milieux marginalisés, et favorisant l'émergence
        d'un réseau de citoyens responsables et engagés.
      </p>
      <ol class="flex list-disc flex-row gap-8">
        <li class="list-none">Pick it</li>
        <li class="">Book it</li>
        <li class="">Groom it</li>
      </ol>
      <button class="btn btn-primary w-auto self-auto">En savoir plus</button>
    </div>
  </div>
</div>
