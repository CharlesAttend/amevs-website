<script>
  let { name, role, status, pp } = $props();
</script>

<div class="card card-side bg-base-100 shadow-sm">
  <figure class="w-1/2 px-2">
    <div class="avatar flex items-center">
      <div class="ring-primary ring-offset-base-100 w-full rounded-full ring ring-offset-2">
        <img src={pp} alt={name} />
      </div>
    </div>
  </figure>
  <div class="card-body w-full">
    <h2 class="card-title text-2xl">{name}</h2>
    <p class="grid grid-cols-2 content-stretch items-stretch gap-1">
      <span class="text-gray-500">Role : </span>
      <span>{role}</span>
    </p>
    <p class="grid grid-cols-2 content-stretch items-stretch gap-1">
      <span class="text-gray-500">Status : </span>
      <span>{status}</span>
    </p>
  </div>
</div>
