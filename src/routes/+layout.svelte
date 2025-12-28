<script lang="ts">
  import "../app.css";
  import Header from "$lib/components/ui/Header.svelte";
  import Footer from "$lib/components/ui/Footer.svelte";
  import favicon from "$lib/assets/logo.svg";

  let { children } = $props();
</script>

<svelte:head>
  <title>Chainpaye</title>
  <link rel="icon" href={favicon} />
  <meta name="description" content="Unlock Borderless Payments With Chainpaye. Add seamless global and on-chain payments to your business with one lightweight integration." />
  <meta property="og:title" content="Chainpaye" />
  <meta property="og:description" content="Unlock Borderless Payments With Chainpaye. Add seamless global and on-chain payments to your business with one lightweight integration." />
  <meta property="og:image" content="https://chainpaye.com/og-image.png" />
  <meta property="og:url" content="https://chainpaye.com" />
  <meta name="twitter:card" content="summary_large_image" />
  <meta name="twitter:title" content="Chainpaye" />
  <meta name="twitter:description" content="Unlock Borderless Payments With Chainpaye. Add seamless global and on-chain payments to your business with one lightweight integration." />
  <meta name="twitter:image" content="https://chainpaye.com/og-image.png" />
</svelte:head>

<main class="font-manrope space-y-24">
  <Header />
  <div class="px-1 md:px-10 lg:px-20 space-y-8 md:space-y-52">
    {@render children()}
  </div>
</main>
<Footer />
