<script>
  import Icon from "@iconify/svelte";
  let currentIndex = $state(1);
  const cards = [
    {
      title: "For Individuals",
      content: "Send and receive money instantly, no extra apps needed.",
      subContent:
        "Pay friends, family, or split bills with ChainPaye fast, secure, and easy.",
    },
    {
      title: "For Businesses",
      content:
        "Leverage our APIs to scale your business while accepting global payments in USD 🇺🇸, EUR 🇪🇺, GBP 🇬🇧 — and more coming soon.",
      subContent:
        "Funds are automatically converted into NGN 🇳🇬, GHS 🇬🇭, or KES 🇰🇪 at real-time rates.",
    },
    {
      title: "For Freelancers & Creators",
      content:
        "Generate a payment link using Chainpaye and get settled in less than a minute.",
      subContent:
        "Clients pay through a bank card or bank transfers for US 🇺🇸 while EUR 🇪🇺 and GBP 🇬🇧 uses Bank card strictly",
    },
  ];
  function next() {
    currentIndex = (currentIndex + 1) % cards.length;
  }
  function previous() {
    currentIndex = (currentIndex - 1 + cards.length) % cards.length;
  }
  function getCardStyle(index) {
    const diff = (index - currentIndex + cards.length) % cards.length;
    if (diff === 0) {
      return "z-30 scale-90 opacity-100 translate-x-0 rotate-0";
    } else if (diff === 1 || diff === -(cards.length - 1)) {
      return "z-20 scale-60 md:scale-70 md:opacity-90 translate-x-64 md:translate-x-90 md:-translate-y-10  md:-rotate-20";
    } else {
      return "z-10 scale-60 md:scale-70 md:opacity-90 -translate-x-64 md:-translate-x-90 md:-translate-y-10 md:rotate-20";
    }
  }
</script>

<div class="flex flex-col items-center justify-center">
  <div class="w-full text-center mb-12">
    <h1 class="text-4xl font-bold text-gray-900 mb-4">
      Real world application
    </h1>
    <p class="text-lg text-gray-600">
      Discover how people and businesses use Chainpaye
    </p>
  </div>
  <div
    class="relative w-full max-w-5xl h-96 mb-1 overflow-hidden lg:overflow-visible"
  >
    {#each cards as card, index}
      <div
        class="absolute inset-0 flex items-center justify-center transition-all duration-500 ease-out {getCardStyle(
          index,
        )}"
      >
        <div class="relative">
          <div
            class="absolute inset-0 bg-gray-300 rounded-3xl transform -translate-y-6"
          ></div>

          <!-- Main Card -->
          <div
            class="relative bg-white rounded-3xl shadow-xl p-8 w-full max-w-md h-72 flex flex-col justify-between"
          >
            <div>
              <h3 class="text-2xl font-semibold text-gray-900 mb-4 italic">
                {card.title}
              </h3>
              <p class="text-gray-700 mb-3 italic">{card.content}</p>
              <p class="text-gray-600 text-sm italic">{card.subContent}</p>
            </div>
          </div>
        </div>
      </div>
    {/each}
  </div>
  <div class="flex gap-4">
    <button
      onclick={previous}
      class="bg-gray-200 text-gray-500 rounded-full p-4 transition-all duration-200 hover:scale-110"
      aria-label="back button"
    >
      <Icon icon="formkit:arrowleft" />
    </button>
    <button
      onclick={next}
      class="bg-gray-200 text-gray-500 rounded-full p-4 transition-all duration-200 hover:scale-110"
      aria-label="next button"
    >
      <Icon icon="formkit:arrowright" />
    </button>
  </div>
</div>
