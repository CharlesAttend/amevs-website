<script>
  import RatingCard from '$lib/component/Rating_Card.svelte';
</script>

<div class="bg-base-200 hero min-h-dvh lg:min-h-auto lg:p-16">
  <div class="hero-content flex-col">
    <div>
      <h1 class="text-5xl font-bold">Témoignages</h1>
    </div>
    <div class="flex grow basis-0 flex-col items-center justify-center gap-4 lg:flex-row">
      <RatingCard
        note="5"
        description="Quand j'ai reçu mon premier violon, j'ai senti que quelqu'un croyait en moi. Aujourd'hui, je peux enfin apprendre et rêver d'un avenir musical."
        name="Jean Dupont"
        location="Paris"
        pp="https://thispersondoesnotexist.com/"
      />
      <RatingCard
        note="4"
        description="Grâce à cette association, j'ai un vrai piano pour m'entraîner. La musique me permet d'oublier les difficultés du quotidien et de me concentrer sur mon avenir."
        name="Jean Dupont"
        location="Paris"
        pp="https://cdn.discordapp.com/avatars/264852636375842816/0030b35e4d7bbfe9b3e03de701f00aed.webp?size=2048&format=webp"
      />
      <RatingCard
        note="4"
        description="Voir ces enfants jouer avec passion grâce aux instruments donnés est un vrai miracle. Merci à tous ceux qui rendent cela possible."
        name="Jean Dupont"
        location="Paris"
        pp="https://cdn.discordapp.com/avatars/622451740947644435/e2512c2afc5f668b0791929ce90ce24d.webp?size=2048&format=webp"
      />
    </div>
  </div>
</div>
