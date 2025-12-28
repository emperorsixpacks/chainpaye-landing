<script lang="ts">
  import Button from '$lib/components/Button.svelte';
  import Logo from '$lib/assets/logo.svg';

  let isOpen = false;

  function toggleMenu() {
    isOpen = !isOpen;
  }
</script>

<header class="relative">
  <nav class="container mx-auto px-6 py-4">
    <div class="flex items-center justify-between">
      <div class="text-xl font-semibold text-gray-700">
        <a href="/" class="text-gray-800 hover:text-gray-700">
          <img src={Logo} alt="ChainPaye Logo" />
        </a>
      </div>
      <div class="hidden items-center space-x-4 md:flex">
        <a href="/for-businesses" class="text-gray-800 hover:text-gray-700">For Businesses</a>
        <a href="/use-cases" class="text-gray-800 hover:text-gray-700">Use cases</a>
        <a href="/about" class="text-gray-800 hover:text-gray-700">About</a>
      </div>
      <div class="hidden items-center space-x-2 md:flex">
        <Button text="Start on WhatsApp" icon="iconoir:whatsapp" />
      </div>
      <div class="flex md:hidden">
        <button on:click={toggleMenu} type="button" class="text-gray-500 hover:text-gray-600 focus:text-gray-600 focus:outline-none">
          <svg viewBox="0 0 24 24" class="h-6 w-6 fill-current">
            {#if isOpen}
              <path
                fill-rule="evenodd"
                clip-rule="evenodd"
                d="M18.278 16.864a1 1 0 0 1-1.414 1.414l-4.829-4.828-4.828 4.828a1 1 0 0 1-1.414-1.414l4.828-4.829-4.828-4.828a1 1 0 0 1 1.414-1.414l4.829 4.828 4.828-4.828a1 1 0 1 1 1.414 1.414l-4.828 4.829 4.828 4.828z"
              />
            {:else}
              <path
                fill-rule="evenodd"
                d="M4 5h16a1 1 0 0 1 0 2H4a1 1 0 1 1 0-2zm0 6h16a1 1 0 0 1 0 2H4a1 1 0 0 1 0-2zm0 6h16a1 1 0 0 1 0 2H4a1 1 0 0 1 0-2z"
              />
            {/if}
          </svg>
        </button>
      </div>
    </div>
  </nav>

  {#if isOpen}
    <div class="fixed inset-0 z-40 bg-black bg-opacity-50 md:hidden" on:click={toggleMenu} />
    <div
      class="fixed right-0 top-0 z-50 h-full w-full transform bg-[#21242c] p-6 shadow-lg transition-transform duration-300 ease-in-out md:hidden"
      class:translate-x-full={!isOpen}
    >
      <div class="flex justify-end">
        <button on:click={toggleMenu} type="button" class="text-gray-400 hover:text-white focus:text-white focus:outline-none">
          <svg viewBox="0 0 24 24" class="h-6 w-6 fill-current">
            <path
              fill-rule="evenodd"
              clip-rule="evenodd"
              d="M18.278 16.864a1 1 0 0 1-1.414 1.414l-4.829-4.828-4.828 4.828a1 1 0 0 1-1.414-1.414l4.828-4.829-4.828-4.828a1 1 0 0 1 1.414-1.414l4.829 4.828 4.828-4.828a1 1 0 1 1 1.414 1.414l-4.828 4.829 4.828 4.828z"
            />
          </svg>
        </button>
      </div>
      <div class="mt-8 flex flex-col items-start space-y-6">
        <a href="/for-businesses" class="text-lg text-gray-200 hover:text-white">For Businesses</a>
        <a href="/use-cases" class="text-lg text-gray-200 hover:text-white">Use cases</a>
        <a href="/about" class="text-lg text-gray-200 hover:text-white">About</a>
        <Button text="Start on WhatsApp" icon="iconoir:whatsapp" />
      </div>
    </div>
  {/if}
</header>
