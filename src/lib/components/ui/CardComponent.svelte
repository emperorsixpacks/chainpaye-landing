<script lang="ts">
  import Button from "$lib/components/Button.svelte";
  import Card1Gradiant from "$lib/assets/images/cards/card_1_gradiant.svg";

  let {
    title,
    imageSrc = "",
    imageAlt = "",
    buttonText,
    buttonIcon,
    buttonHref = "/",
    buttonSwap = false,
    swap = false,
    extraStyle = "",
    sectionClass = "",
    titleClass = "",
    descriptionClass = "",
    containerClass = "",
    description,
  }: {
    title: string;
    imageSrc?: string;
    imageAlt?: string;
    buttonText: string;
    buttonIcon: string;
    buttonHref?: string;
    buttonSwap?: boolean;
    swap?: boolean;
    extraStyle?: string;
    sectionClass?: string;
    titleClass?: string;
    descriptionClass?: string;
    containerClass?: string;
    description?: import("svelte").Snippet;
  } = $props();
</script>

<section class={`${sectionClass} lg:rounded-4xl overflow-hidden relative`}>
  <div class={`px-4 md:px-8 lg:px-2 py-12 lg:py-18 ${containerClass}`}>
    <div
      class="flex flex-col-reverse gap-8 lg:gap-16 lg:flex-row justify-center"
    >
      <!-- Image Side -->
      <div class="w-full lg:w-1/2" class:lg:order-last={!swap}>
        <div class={`relative w-full max-w-md lg:max-w-lg ${extraStyle}`}>
          <img
            src={imageSrc}
            alt={imageAlt}
            class="w-full h-auto transform lg:rotate-6 lg:scale-150"
          />
          <div
            class="absolute inset-0 m-auto"
          >
            <img src={Card1Gradiant} alt={title} />
          </div>
        </div>
      </div>
      <!-- Content Side -->
      <div class="w-full lg:w-1/2 space-y-6 md:space-y-8 lg:pr-25">
        <h2
          class={`text-3xl md:text-4xl lg:text-5xl font-bold leading-tight ${titleClass}`}
        >
          {@html title}
        </h2>

        <div
          class={`text-base md:text-lg lg:text-xl leading-relaxed lg:pr-28 ${descriptionClass}`}
        >
          {#if description}
            {@render description()}
          {/if}
        </div>

        <div class="pt-4">
          <Button
            text={buttonText}
            icon={buttonIcon}
            swap={buttonSwap}
            url={buttonHref}
          />
        </div>
      </div>
    </div>
  </div>
</section>
