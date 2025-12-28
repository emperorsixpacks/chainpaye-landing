<script lang="ts">
  import FeatureSection from "$lib/components/ui/FeatureSection.svelte";
  import WhatappMockup from "$lib/assets/images/whatsapp_mockup.svg";
</script>

<FeatureSection
  sectionClass="bg-[#E8EDFF]"
  title="Send and receive Money<br /> instantly on <span class='font-bold'>Whatsapp</span>"
  titleClass="font-semibold text-gray-800 leading-10"
  descriptionClass="text-gray-600 leading-6"
  buttonText="Start on WhatsApp"
  buttonHref="https://wa.link/m25oou"
  buttonIcon="iconoir:whatsapp"
  imageSrc={WhatappMockup}
  imageAlt="Send and receive money instantly on Whatsapp"
  extraStyle="lg:transform lg:-translate-y-[62%] lg:translate-x-[10%]"
  swap={true}
>
  <div slot="description">
    <p>
      With Chainpaye, anyone can send or receive money globally and withdraw to
      their local bank or mobile money — all inside a WhatsApp chat.
    </p>
  </div>
</FeatureSection>
