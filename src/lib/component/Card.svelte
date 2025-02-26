<script>
  let {
    title = 'Card Title',
    description = 'A card component has a figure, a body part, and inside body there are title and actions parts',
    img = 'https://img.daisyui.com/images/stock/photo-1606107557195-0e29a4b5b4aa.webp',
    alt,
    button_text = '',
    button_href = '#'
  } = $props();
  // w-96
</script>

<div class="card-sm bg-base-100 shadow-sm lg:card-lg w-full h-full">
  <figure class="w-full h-1/2 overflow-hidden">
    <img class="min-w-full min-h-full" src={img} alt={title} />
  </figure>
  <div class="card-body h-1/2">
    <h2 class="card-title">{title}</h2>
    <p>
      {description}
    </p>
    {#if button_text != ''}
      <div class="card-actions justify-end">
        <a href={button_href} class="btn btn-primary">{button_text}</a>
      </div>
    {/if}
  </div>
</div>
