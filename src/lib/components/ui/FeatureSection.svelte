<script lang="ts">
  import Button from "$lib/components/Button.svelte";

  export let title: string;
  export let imageSrc = "";
  export let imageAlt = "";
  export let buttonText: string;
  export let buttonIcon: string;
  export let buttonHref = "/";
  export let buttonSwap = false;
  export let swap = false;
  export let extraStyle = "";

  // Allow passing down classes
  export let sectionClass = "";
  export let titleClass = "";
  export let descriptionClass = "";
  export let containerClass = "";
</script>

<section class={`${sectionClass} md:rounded-4xl overflow-hidden `}>
  <div class={`px-4 lg:px-16 pt-12 lg:py-28 ${containerClass}`}>
    <div class="flex flex-col-reverse px-9 gap-8 lg:gap-16 md:flex-row">
      <div class="w-full md:w-1/2 justify-center" class:md:order-last={!swap}>
        <div class={`lg:absolute w-full max-w-md lg:max-w-lg ${extraStyle}`}>
          <img src={imageSrc} alt={imageAlt} class="w-full h-auto" />
        </div>
      </div>

      <!-- Content Side -->
      <div class="w-full md:w-1/2 space-y-6 md:space-y-8">
        <h2
          class={`text-3xl md:text-4xl font-bold leading-tight ${titleClass}`}
        >
          {@html title}
        </h2>

        <div
          class={`text-base md:text-lg lg:text-xl lg:pr-70 leading-relaxed ${descriptionClass}`}
        >
          <slot name="description" />
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

<style>
  /* Optional: Add custom styles if needed */
</style>
