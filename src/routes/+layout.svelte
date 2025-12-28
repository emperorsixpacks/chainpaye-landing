<script lang="ts">
  import "../app.css";
  import Header from "$lib/components/ui/Header.svelte";
  import Footer from "$lib/components/ui/Footer.svelte";

  let { children } = $props();
</script>

<main class="font-manrope space-y-24">
  <Header />
  <div class="px-1 md:px-10 lg:px-20 space-y-8 md:space-y-52">
    {@render children()}
  </div>
</main>
<Footer />
