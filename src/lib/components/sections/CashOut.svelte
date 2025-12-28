<script lang="ts">
  import FeatureSection from "$lib/components/ui/FeatureSection.svelte";
  import WhatsappMockup from "$lib/assets/images/whatsapp_mockup_2.svg";
</script>

<FeatureSection
  sectionClass="bg-[#E8EDFF]"
  title="Cash out crypto directly from WhatsApp."
  titleClass="font-bold text-gray-800"
  descriptionClass="text-gray-600"
  buttonText="Start on WhatsApp"
  buttonIcon="iconoir:whatsapp"
  imageSrc={WhatsappMockup}
  imageAlt="Cash out crypto directly from WhatsApp"
  extraStyle="lg:transform lg:-translate-y-[68%]"
  swap={false}
>
  <div slot="description">
    <p>Send crypto, confirm once, and receive money in your Bank account.</p>
  </div>
</FeatureSection>
