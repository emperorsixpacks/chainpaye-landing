<script lang="ts">
  import Hero from "$lib/components/sections/Hero.svelte";
  import SendAndReceive from "$lib/components/sections/SendAndReceive.svelte";
  import CashOut from "$lib/components/sections/CashOut.svelte";
  import SpendStablecoins from "$lib/components/sections/SpendStablecoins.svelte";
  import GetStarted from "$lib/components/sections/GetStarted.svelte";
  import TransformingPayments from "$lib/components/sections/TransformingPayments.svelte";
  import RealWorld from "$lib/components/sections/RealWorld.svelte";
  import PaymentAPIs from "$lib/components/sections/PaymentAPIs.svelte";
</script>

<div class="lg:space-y-60">
  <div class="lg:space-y-80">
    <Hero />
    <div class="lg:space-y-100">
      <SendAndReceive />
      <CashOut />
    </div>
  </div>
</div>
<SpendStablecoins />
<div class="p-2">
  <GetStarted />
  <TransformingPayments />
  <RealWorld />
</div>
<!-- <PaymentAPIs /> -->
