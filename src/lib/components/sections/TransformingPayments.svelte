<script lang="ts">
  import Whatsapp from "$lib/assets/images/whatsapp.svg";
  import Apikey from "$lib/assets/images/apikey.svg";
  import Support from "$lib/assets/images/support.svg";
  import Features from "$lib/assets/images/features.svg";
  import Receive from "$lib/assets/images/receive.png";

  const services = [
    {
      title: "Seamless WhatsApp Payments",
      description:
        "Send and receive payments inside WhatsApp — chat, tap, done.",
      component: Whatsapp,
    },
    {
      title: "Global Payment API",
      description:
        "Accept global payments easily and focus on growth with quick Chainpaye integration.",
      component: Apikey,
    },
    {
      title: "Multi-Currency Support",
      description:
        "Receive funds in NGN, GHS, ZAR, KES, USD and convert seamlessly.",
      component: Receive,
    },
    {
      title: "24/7 customer support",
      description:
        "Our customer support team is readily available to assist you whenever needed.",
      component: Support,
    },
  ];
</script>

<section class="space-y-8 py-8">
  <div class="space-y-6 text-center text-black px-2">
    <h3 class="text-4xl leading-10 lg:px-87.5 lg:text-6xl lg:leading-14">
      Transforming cross-border payments in Africa
    </h3>
    <span class="text-lg text-gray-500 lg:text-3xl"
      >Simple instant and low fees</span
    >
  </div>
  <div class="grid grid-cols-1 items-stretch gap-16 lg:grid-cols-[3fr_7fr]">
    <div
      class="bg-linear-to-b from-blue-600 to-blue-950 rounded-3xl grid grid-rows-[1fr_2fr] gap-3"
    >
      <div
        class="relative flex flex-wrap items-center justify-center pb-20 row-start-2"
      >
        <img src={Features} alt="Features" />
      </div>
    </div>

    <!-- Right Column -->

    <div
      class="relative grid grid-cols-1 sm:grid-cols-2 rounded-3xl overflow-hidden"
    >
      <div
        class="hidden sm:block absolute inset-y-0 left-1/2 w-px bg-gray-300"
      ></div>
      <div class="absolute inset-x-0 top-1/2 h-px bg-gray-300"></div>

      {#each services as service}
        <div class="flex h-full flex-col justify-center p-10 space-y-3">
          <img src={service.component} alt={service.title} class="max-w-full" />

          <h3 class="text-md font-bold text-gray-800">
            {service.title}
          </h3>

          <p class="text-sm text-gray-600 leading-relaxed">
            {service.description}
          </p>
        </div>
      {/each}
    </div>
  </div>
</section>
