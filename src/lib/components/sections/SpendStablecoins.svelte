<script lang="ts">
  import CardComponent from "$lib/components/ui/CardComponent.svelte";
  import Card1 from "$lib/assets/images/cards/card_1.png";
</script>

<CardComponent
  sectionClass="bg-[#300026] text-white"
  title="Spend your stablecoins like cash – anywhere Visa works"
  titleClass="font-bold leading-10"
  buttonText="Preorder now"
  buttonIcon="lucide:arrow-right"
  buttonSwap={true}
  imageSrc={Card1}
  imageAlt="Spend your stablecoins like cash"
  swap={true}
>
  {#snippet description()}
    <p class="mt-4">
      Spend your stablecoins like cash in over 80+ countries including EUR, USD,
      NGN, KSH🇬🇧🇺🇸🇳🇬
    </p>
    <p class="mt-4">No need for Offramps</p>
  {/snippet}
</CardComponent>
