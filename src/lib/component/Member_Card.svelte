<script>
  let { name, role, status, pp } = $props();
</script>

<div class="card card-side bg-base-100 shadow-sm">
  <div class="card-body w-full flex-row gap-5 p-5 items-center">
    <figure class="w-1/2">
      <div class="avatar flex items-center">
        <div class="ring-primary ring-offset-base-100 w-full rounded-full ring ring-offset-2">
          <img src={pp} alt={name} />
        </div>
      </div>
    </figure>
    <div class="flex w-1/2 flex-col gap-2">
      <h2 class="card-title text-2xl">{name}</h2>
      <p class="my-2 flex flex-col gap-1 text-base lg:text-lg">
        <!-- <span class="text-gray-500">Role :</span> -->
        <span>{role}</span>
        <span class="divider m-0"></span>
        <!-- <span class="text-gray-500">Status :</span> -->
        <span>{status}</span>
      </p>
    </div>
  </div>
</div>
