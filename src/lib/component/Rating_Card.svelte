<script>
  let {
    note = 5,
    description = 'A card component has a figure, a body part, and inside body there are title and actions parts',
    name = 'Jean Dupont',
    location = 'Paris',
    pp = ''
  } = $props();
  let stars = Array.from({ length: note }, (_, i) => i < note);
  import star_svg from '$lib/assets/star.svg';
</script>

<div class="card bg-base-200 shadow-lg">
  <div class="card-body">
    <div class="badge badge-primary p-1">
      {#each stars as star}
        <img class="h-full" src={star_svg} alt="star" />
      {/each}
    </div>
    <p>
      {description}
    </p>
    <div class="flex items-center justify-start gap-4">
      <figure>
        <div class="avatar w-12 pl-0">
          <div class="ring-primary ring-offset-base-100 w-24 rounded-full ring ring-offset-2">
            <img src={pp} alt={name} />
          </div>
        </div>
      </figure>
      <div>
        <h4 class="card-title text-primary text-sm font-bold">
          {name}
        </h4>
        <div class="badge badge-secondary badge-sm">{location}</div>
      </div>
    </div>
  </div>
</div>
