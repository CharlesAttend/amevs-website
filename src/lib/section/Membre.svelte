<script>
  import MemberCard from '$lib/component/Member_Card.svelte';
</script>

<div class="bg-base-200 hero min-h-screen">
  <div class="hero-content flex-col lg:flex-row">
    <div>
      <h1 class="text-5xl font-bold">Membres de l'association</h1>
      <!-- <button>Vois tous nos projets</button> -->
    </div>
    <div class="flex flex-col gap-4">
      <MemberCard
        name="Jéricho Pierre-Noël"
        role="Président"
        status="Étudiant en informatique"
        pp="https://thispersondoesnotexist.com/"
      />
      <MemberCard
        name="Sohann"
        role="Responsable communiquation"
        status="Étudiante"
        pp="https://thispersondoesnotexist.com"
      />
      <MemberCard
        name="Mélissa"
        role="Trésorière"
        status="Étudiante"
        pp="https://thispersondoesnotexist.com"
      />
      <MemberCard
        name="Cécilia"
        role="Responsable des partenariats"
        status="Étudiante"
        pp="https://thispersondoesnotexist.com"
      />
    </div>
    <button class="btn btn-primary">Voir tous les membres</button>
  </div>
</div>
