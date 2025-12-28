<script lang="ts">
  import FeatureSection from '$lib/components/ui/FeatureSection.svelte';
  import SpendStablecoinsImage from '$lib/assets/images/support.svg';
</script>

<FeatureSection
  sectionClass="bg-[#300026] text-white"
  title="Spend your stablecoins like cash – anywhere Visa works"
  titleClass="font-semibold leading-10"
  buttonText="Preorder now"
  buttonIcon="lucide:arrow-right"
  buttonSwap={true}
  imageSrc={SpendStablecoinsImage}
  imageAlt="Spend your stablecoins like cash"
  swap={true}
>
  <div slot="description">
    <p class="mt-4">
      Spend your stablecoins like cash in over 80+ countries including EUR, USD, NGN, KSH🇬🇧🇺🇸🇳🇬
    </p>
    <p class="mt-4">No need for Offramps</p>
  </div>
</FeatureSection>
