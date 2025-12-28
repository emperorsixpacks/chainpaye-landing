<script lang="ts">
  import CountiesLarge from "$lib/assets/images/countries_large.svg";
  import CountiesSmall from "$lib/assets/images/countries_small.svg";
  import WalletLarge from "$lib/assets/images/wallet_large.svg";
  import WalletSmall from "$lib/assets/images/wallet_small.svg";
  import DemoSmall from "$lib/assets/images/demo_small.svg";
  import DemoLarge from "$lib/assets/images/demo_large.svg";
  const steps = [
    {
      stepNumber: "Step 1",
      title: "Start a WhatsApp Chat",
      imageSmall: DemoSmall,
      imageLarge: DemoLarge,
      swap: false,
      items: [
        'Click <a href="/" class="text-[#0066FF] underline">here</a> to get directed to our WhatsApp AI agent',
        "Our AI Agent greets you instantly – no app download required",
        "Verify your identity securely inside WhatsApp",
      ],
    },
    {
      stepNumber: "Step 2",
      title: "Create Your Wallet",
      imageSmall: WalletSmall,
      imageLarge: WalletLarge,
      swap: true,
      items: [
        "Follow the prompts to create your Chainpaye wallet in seconds",
        "Set your 4-digit PIN for secure transactions.",
        "Your wallet is instantly ready for global payments",
      ],
    },
    {
      stepNumber: "Step 3",
      title: "Start sending & receiving payments globally",
      imageLarge: CountiesLarge,
      imageSmall: CountiesSmall,
      swap: false,
      items: [
        "Chat, send, and receive money directly inside WhatsApp.",
        "Pay or get paid in multiple currencies – USD, EUR, GBP, NGN, and <br>more.",
        "Track every transaction in real-time through the WhatsApp <br>interface.",
      ],
    },
  ];
</script>

<section class="space-y-12">
  <div class="space-y-4 text-center text-gray-500">
    <h3 class="text-4xl leading-10 md:hidden">
      Get started with Chainpaye in
      <span class="text-black">Three Simple Steps</span>
    </h3>
    <h3 class="text-5xl leading-14 hidden md:block">
      Get started with Chainpaye in<br />
      <span class="text-black">Three Simple Steps</span>
    </h3>
    <span class="md:lg"
      >Join Chainpaye in minutes and start receiving payments globally</span
    >
  </div>
  <div class="flex flex-col gap-y-16 text-left lg:gap-y-24">
    {#each steps as step, i}
      <div
        class="flex flex-col gap-x-8 gap-y-8 rounded-4xl bg-white p-3 lg:flex-row lg:gap-x-8"
      >
        <div class="flex-1 text-left p-4" class:md:order-last={step.swap}>
          <p class="font-medium text-[#0066FF]">{step.stepNumber}</p>
          <h3
            class="mt-4 text-2xl font-medium leading-[120%] tracking-[-1.5%] text-black md:text-4xl"
          >
            {step.title}
          </h3>
          <ul class="mt-8 flex flex-col gap-y-4">
            {#each step.items as item, j}
              <li class="flex items-start gap-x-4">
                <span
                  class="flex h-8 w-8 items-center justify-center rounded-full bg-[#E5F0FF] font-medium text-[#0066FF] md:text-lg"
                >
                  {j + 1}
                </span>
                <span class="flex-1 text-gray-600 text-sm md:text-xl">
                  {@html item}
                </span>
              </li>
            {/each}
          </ul>
        </div>
        <img src={step.imageSmall} alt={step.title} class="md:hidden" />
        <img src={step.imageLarge} alt={step.title} class="hidden md:block" />
      </div>
    {/each}
  </div>
</section>
