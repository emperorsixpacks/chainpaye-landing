<script lang="ts">
  import Button from "$lib/components/Button.svelte";
  import HeroMobile from "$lib/assets/images/hero_mobile.svg";
  import HeroDesktop from "$lib/assets/images/hero_desktop.svg";
</script>

<section class="font-manrope space-y-10 md:min-h-screen">
  <div class="text-center">
    <h1 class="text-3xl text-center font-semibold text-gray-900 md:hidden">
      Pay, Send and Receive Money globally as simple as a chat.
    </h1>

    <h1
      class="text-5xl text-center font-semibold text-gray-900 hidden md:block"
    >
      Pay, Send and Receive <br />Money globally as simple as a chat.
    </h1>

    <p class="mt-4 text-lg text-gray-600 md:hidden">
      Send and receive money worldwide— instantly on WhatsApp
    </p>

    <p class="mt-4 text-lg text-gray-600 md:text-xl hidden md:block">
      Send and receive money worldwide — instantly on WhatsApp
    </p>

    <div class="mt-8">
      <Button text="Start on WhatsApp" icon="iconoir:whatsapp" />
    </div>
  </div>
  <div>
    <img src={HeroMobile} class="w-full lg:hidden" alt="hero" />
    <img src={HeroDesktop} class="hidden lg:w-full lg:block" alt="hero" />
  </div>
</section>
