<script lang="ts">
  import Button from "$lib/components/Button.svelte";
</script>

<div class="flex flex-col mt-20 lg:space-y-18">
  <div class="flex-1 flex px-4 justify-between lg:px-20">
    <div class="w-full grid md:grid-cols-2 gap-5">
      <div
        class="lg:pr-20 md:space-y-2 leading-12 lg:leading-16 tracking-[-1%] font-medium text-gray-900"
      >
        <h1 class="text-3xl md:text-3xl lg:text-6xl">
          Unlock Borderless Payments With Chainpaye
        </h1>
        <h6>
          Message support at <a href="mailto:business@chainpaye.com"
            >business@chainpaye.com</a
          >
        </h6>
      </div>
      <div class="lg:pl-90">
        <p class="text-gray-600 mb-6 leading-relaxed">
          Add seamless global and on-chain payments to your business with one
          lightweight integration — we handle compliance, settlement, liquidity,
          and infrastructure so you can focus on growth.
        </p>
        <Button
          text="Get in touch with us"
          icon="lucide:arrow-right"
          swap={true}
        />
      </div>
      <div class="flex items-center gap-2 md:hidden">
        <a
          href="https://wa.link/m25oou"
          target="_blank"
          class="w-8 h-8 rounded-full bg-gray-600 hover:bg-gray-700 flex items-center justify-center transition"
          aria-label="whatsapp"
        >
          <svg
            class="w-5 h-5 text-white"
            fill="currentColor"
            viewBox="0 0 24 24"
          >
            <path
              d="M17.472 14.382c-.297-.149-1.758-.867-2.03-.967-.273-.099-.471-.148-.67.15-.197.297-.767.966-.94 1.164-.173.199-.347.223-.644.075-.297-.15-1.255-.463-2.39-1.475-.883-.788-1.48-1.761-1.653-2.059-.173-.297-.018-.458.13-.606.134-.133.298-.347.446-.52.149-.174.198-.298.298-.497.099-.198.05-.371-.025-.52-.075-.149-.669-1.612-.916-2.207-.242-.579-.487-.5-.669-.51-.173-.008-.371-.01-.57-.01-.198 0-.52.074-.792.372-.272.297-1.04 1.016-1.04 2.479 0 1.462 1.065 2.875 1.213 3.074.149.198 2.096 3.2 5.077 4.487.709.306 1.262.489 1.694.625.712.227 1.36.195 1.871.118.571-.085 1.758-.719 2.006-1.413.248-.694.248-1.289.173-1.413-.074-.124-.272-.198-.57-.347m-5.421 7.403h-.004a9.87 9.87 0 01-5.031-1.378l-.361-.214-3.741.982.998-3.648-.235-.374a9.86 9.86 0 01-1.51-5.26c.001-5.45 4.436-9.884 9.888-9.884 2.64 0 5.122 1.03 6.988 2.898a9.825 9.825 0 012.893 6.994c-.003 5.45-4.437 9.884-9.885 9.884m8.413-18.297A11.815 11.815 0 0012.05 0C5.495 0 .16 5.335.157 11.892c0 2.096.547 4.142 1.588 5.945L.057 24l6.305-1.654a11.882 11.882 0 005.683 1.448h.005c6.554 0 11.89-5.335 11.893-11.893a11.821 11.821 0 00-3.48-8.413z"
            />
          </svg>
        </a>
        <a
          href="https://x.com/chainpaye"
          target="_blank"
          class="w-8 h-8 rounded-full bg-gray-600 hover:bg-gray-700 flex items-center justify-center transition"
          aria-label="twitter"
        >
          <svg
            class="w-5 h-5 text-white"
            fill="currentColor"
            viewBox="0 0 24 24"
          >
            <path
              d="M18.244 2.25h3.308l-7.227 8.26 8.502 11.24H16.17l-5.214-6.817L4.99 21.75H1.68l7.73-8.835L1.254 2.25H8.08l4.713 6.231zm-1.161 17.52h1.833L7.084 4.126H5.117z"
            />
          </svg>
        </a>
        <a
          href="https://chat.whatsapp.com/JacU3p0Aiwy1sQ00YRoXeS"
          target="_blank"
          class="w-8 h-8 rounded-full bg-gray-600 hover:bg-gray-700 flex items-center justify-center transition"
          aria-label="whatsapp-group"
        >
          <svg
            class="w-5 h-5 text-white"
            fill="currentColor"
            viewBox="0 0 24 24"
          >
            <path
              d="M16 11.37A4 4 0 1 1 11.37 16 4 4 0 0 1 16 11.37zM16 8a3 3 0 1 0 0 6 3 3 0 0 0 0-6zm-4.75 10a1.25 1.25 0 1 1-1.25-1.25A1.25 1.25 0 0 1 11.25 18zM19 18a1.25 1.25 0 1 1-1.25-1.25A1.25 1.25 0 0 1 19 18zM6 18a1.25 1.25 0 1 1-1.25-1.25A1.25 1.25 0 0 1 6 18zM12 2a10 10 0 1 0 0 20 10 10 0 0 0 0-20zM12 4a8 8 0 1 1 0 16 8 8 0 0 1 0-16z"
            />
          </svg>
        </a>
      </div>
    </div>
  </div>

  <hr class="border-t border-gray-300 mt-4 md:hidden" />
  <!-- Footer -->
  <footer class="bg-linear-to-b from[#F5F5F5] to-blue-200">
    <div class="max-w-full p-2 md:px-10 lg:px-20">
      <nav
        class="flex flex-col md:justify-between md:flex-row gap-5 text-gray-700"
      >
        <div class="flex flex-col md:flex-row gap-5 md:gap-10">
          <a href="#solutions" class="hover:text-gray-900 transition"
            >Solutions</a
          >
          <a href="#developers" class="hover:text-gray-900 transition"
            >Developers</a
          >
          <a href="#use-cases" class="hover:text-gray-900 transition"
            >Use cases</a
          >
          <!-- <div class="flex items-center gap-2">
            <span class="text-gray-700">Theme</span>
            <button
              class="w-8 h-8 rounded-full bg-white shadow flex items-center justify-center"
            >
              <span class="text-lg">☀️</span>
            </button>
            <button
              class="w-8 h-8 rounded-full bg-gray-600 shadow flex items-center justify-center"
            >
              <span class="text-lg">🌙</span>
            </button>
          </div> -->
        </div>
        <div class="gap-2 hidden md:flex">
          <a
            href="https://chat.whatsapp.com/JacU3p0Aiwy1sQ00YRoXeS"
            target="_blank"
            class="w-8 h-8 rounded-full bg-gray-600 hover:bg-gray-700 flex items-center justify-center transition"
            aria-label="whatsapp-group"
          >
            <svg
              class="w-5 h-5 text-white"
              fill="currentColor"
              viewBox="0 0 24 24"
            >
              <path
                d="M16 11.37A4 4 0 1 1 11.37 16 4 4 0 0 1 16 11.37zM16 8a3 3 0 1 0 0 6 3 3 0 0 0 0-6zm-4.75 10a1.25 1.25 0 1 1-1.25-1.25A1.25 1.25 0 0 1 11.25 18zM19 18a1.25 1.25 0 1 1-1.25-1.25A1.25 1.25 0 0 1 19 18zM6 18a1.25 1.25 0 1 1-1.25-1.25A1.25 1.25 0 0 1 6 18zM12 2a10 10 0 1 0 0 20 10 10 0 0 0 0-20zM12 4a8 8 0 1 1 0 16 8 8 0 0 1 0-16z"
              />
            </svg>
          </a>
          <a
            href="https://x.com/chainpaye"
            target="_blank"
            class="w-8 h-8 rounded-full bg-gray-600 hover:bg-gray-700 flex items-center justify-center transition"
            aria-label="twitter"
          >
            <svg
              class="w-5 h-5 text-white"
              fill="currentColor"
              viewBox="0 0 24 24"
            >
              <path
                d="M18.244 2.25h3.308l-7.227 8.26 8.502 11.24H16.17l-5.214-6.817L4.99 21.75H1.68l7.73-8.835L1.254 2.25H8.08l4.713 6.231zm-1.161 17.52h1.833L7.084 4.126H5.117z"
              />
            </svg>
          </a>
          <a
            href="https://chat.whatsapp.com/JacU3p0Aiwy1sQ00YRoXeS"
            target="_blank"
            class="w-8 h-8 rounded-full bg-gray-600 hover:bg-gray-700 flex items-center justify-center transition"
            aria-label="whatsapp"
          >
            <svg
              class="w-5 h-5 text-white"
              fill="currentColor"
              viewBox="0 0 24 24"
            >
              <path
                d="M17.472 14.382c-.297-.149-1.758-.867-2.03-.967-.273-.099-.471-.148-.67.15-.197.297-.767.966-.94 1.164-.173.199-.347.223-.644.075-.297-.15-1.255-.463-2.39-1.475-.883-.788-1.48-1.761-1.653-2.059-.173-.297-.018-.458.13-.606.134-.133.298-.347.446-.52.149-.174.198-.298.298-.497.099-.198.05-.371-.025-.52-.075-.149-.669-1.612-.916-2.207-.242-.579-.487-.5-.669-.51-.173-.008-.371-.01-.57-.01-.198 0-.52.074-.792.372-.272.297-1.04 1.016-1.04 2.479 0 1.462 1.065 2.875 1.213 3.074.149.198 2.096 3.2 5.077 4.487.709.306 1.262.489 1.694.625.712.227 1.36.195 1.871.118.571-.085 1.758-.719 2.006-1.413.248-.694.248-1.289.173-1.413-.074-.124-.272-.198-.57-.347m-5.421 7.403h-.004a9.87 9.87 0 01-5.031-1.378l-.361-.214-3.741.982.998-3.648-.235-.374a9.86 9.86 0 01-1.51-5.26c.001-5.45 4.436-9.884 9.888-9.884 2.64 0 5.122 1.03 6.988 2.898a9.825 9.825 0 012.893 6.994c-.003 5.45-4.437 9.884-9.885 9.884m8.413-18.297A11.815 11.815 0 0012.05 0C5.495 0 .16 5.335.157 11.892c0 2.096.547 4.142 1.588 5.945L.057 24l6.305-1.654a11.882 11.882 0 005.683 1.448h.005c6.554 0 11.89-5.335 11.893-11.893a11.821 11.821 0 00-3.48-8.413z"
              />
            </svg>
          </a>
        </div>
      </nav>

      <div class="mb-8">
        <div
          class="text-[58px] md:text-[150px] lg:text-[290px] font-extrabold text-gray-300 opacity-50 select-none tracking-[3%] leading-[100%]"
        >
          <h2
            class="bg-linear-to-t from[#F5F5F5] to-blue-300 bg-clip-text text-transparent"
          >
            CHAINPAYE
          </h2>
        </div>
      </div>

      <!-- Copyright -->
      <div
        class="flex flex-col md:flex-row justify-between text-gray-600 text-sm mb-2"
      >
        <p>©2025 Chainpaye</p>
        <p>All Rights Reserved.</p>
      </div>
    </div>
  </footer>
</div>
