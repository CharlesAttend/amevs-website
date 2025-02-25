<script>
  let { name, role, status, pp } = $props();
</script>

<div class="card card-side bg-base-100 shadow-sm">
  <div class="card-body flex-row gap-5 items-center w-full">
    <figure class="w-1/2">
      <div class="avatar flex items-center">
        <div class="ring-primary ring-offset-base-100 w-full rounded-full ring ring-offset-2">
          <img src={pp} alt={name} />
        </div>
      </div>
    </figure>
    <div class="w-1/2">
      <h2 class="card-title text-2xl">{name}</h2>
      <p class="my-2 grid grid-cols-3 grid-rows-2 content-stretch items-stretch gap-1">
        <span class="text-gray-500">Role : </span>
        <span class="col-span-2">{role}</span>
        <span class="text-gray-500">Status : </span>
        <span class="col-span-2">{status}</span>
      </p>
    </div>
  </div>
</div>
