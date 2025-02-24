<script>
  let { name, role, status, pp } = $props();
</script>

<div class="card card-side bg-base-100 p-4 shadow-sm">
  <figure class="w-1/2">
    <div class="avatar flex items-center">
      <div class="ring-primary ring-offset-base-100 w-full rounded-full ring ring-offset-2">
        <img src={pp} alt={name} />
      </div>
    </div>
  </figure>
  <div class="card-body w-full">
    <h2 class="card-title">{name}</h2>
    <p>{role}</p>
    <p>{status}</p>
  </div>
</div>
