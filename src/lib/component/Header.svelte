<script>
  import { scrollTo } from 'svelte-scrolling';
  import LogoAmevs from '$lib/assets/logos/logo_amevs.svelte';

  let mobile_open = $state(false);
  let menu_item = [
    { title: 'Présentation', name: 'presentation' },
    { title: 'Projets', name: 'project' },
    { title: 'Réalisations', name: 'realisation' },
    { title: 'Nous suivre', name: 'socialslinks' }
  ];
  function closeMenu() {
    mobile_open = false;
  }
</script>

<header class="bg-base-100 fixed z-10 w-full">
  <nav class="mx-auto flex max-w-7xl items-center justify-between p-6 lg:px-8" aria-label="Global">
    <div class="flex lg:flex-1">
      <a href="/" class="p-1.5">
        <span class="sr-only">AMEVS</span>
        <LogoAmevs classAttributes="fill-current w-8" />
      </a>
    </div>
    <div class="flex lg:hidden">
      <button
        type="button"
        class="-m-2.5 inline-flex items-center justify-center rounded-md p-2.5 text-gray-700"
        onclick={() => (mobile_open = true)}
      >
        <span class="sr-only">Open main menu</span>
        <svg
          class="size-6"
          fill="none"
          viewBox="0 0 24 24"
          stroke-width="1.5"
          stroke="currentColor"
          aria-hidden="true"
          data-slot="icon"
        >
          <path
            stroke-linecap="round"
            stroke-linejoin="round"
            d="M3.75 6.75h16.5M3.75 12h16.5m-16.5 5.25h16.5"
          />
        </svg>
      </button>
    </div>
    <div class="hidden lg:flex lg:gap-x-12">
      {#each menu_item as item}
        <a
          href="#{item.name}"
          use:scrollTo={item.name}
          class="text-sm/6 font-semibold text-gray-900">{item.title}</a
        >
      {/each}
    </div>
    <!-- <div class="hidden lg:flex lg:flex-1 lg:justify-end">
			<a href="#" class="text-sm/6 font-semibold text-gray-900"
				>Log in <span aria-hidden="true">&rarr;</span></a
			>
		</div> -->
  </nav>

  <!-- Mobile menu, show/hide based on menu open state. -->
  <div class="lg:hidden {mobile_open ? '' : 'hidden'}" role="dialog" aria-modal="true">
    <!-- Background backdrop, show/hide based on slide-over state. -->
    <div class="fixed inset-0 z-10"></div>
    <div
      class="fixed inset-y-0 right-0 z-10 w-full overflow-y-auto bg-base-100 px-6 py-6 sm:max-w-sm sm:ring-1 sm:ring-gray-900/10"
    >
      <div class="flex items-center justify-between">
        <a href="/" class="p-1.5">
          <span class="sr-only">AMEVS</span>
          <LogoAmevs classAttributes="fill-current w-8" />
        </a>
        <button type="button" class="-m-2.5 rounded-md p-2.5 text-gray-700" onclick={closeMenu}>
          <span class="sr-only">Close menu</span>
          <svg
            class="size-6"
            fill="none"
            viewBox="0 0 24 24"
            stroke-width="1.5"
            stroke="currentColor"
            aria-hidden="true"
            data-slot="icon"
          >
            <path stroke-linecap="round" stroke-linejoin="round" d="M6 18 18 6M6 6l12 12" />
          </svg>
        </button>
      </div>
      <div class="mt-6 flow-root">
        <div class="-my-6 divide-y divide-gray-500/10">
          <div class="space-y-2 py-6">
            <div class="-mx-3">
              {#each menu_item as item}
                <button
                  use:scrollTo={item.name}
                  onclick={closeMenu}
                  class="-mx-3 block rounded-lg px-3 py-2 text-base/7 font-semibold text-gray-900 hover:bg-gray-50"
                >
                  {item.title}
                </button>
              {/each}
            </div>
          </div>
          <!-- <div class="py-6">
						<button class="btn">Button</button>
						<a
							href="#"
							class="-mx-3 block rounded-lg px-3 py-2.5 text-base/7 font-semibold text-gray-900 hover:bg-gray-50"
							>Log in</a
						>
					</div> -->
        </div>
      </div>
    </div>
  </div>
</header>
