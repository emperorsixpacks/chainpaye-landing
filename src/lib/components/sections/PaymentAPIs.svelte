<script lang="ts">
  import Button from "$lib/components/Button.svelte";
  import GearIcon from "$lib/assets/images/noto_gear.svg";
  import CodeBrackets from "$lib/assets/images/code_brackets.svg";
  import StopWatch from "$lib/assets/images/noto-v1_stopwatch.svg";
  import CodeComponeent from "$lib/components/ui/CodeComponeent.svelte";
</script>

<div class="space-y-16">
  <div class="pr-10 md:pr-70 lg:pr-250 hidden lg:block">
    <h2
      class="text-3xl lg:text-6xl text-gray-800 md:text-4xl tracking-[-1%] leading-10.5 lg:leading-12 font-medium"
    >
      Get ready to scale with our payment APIs
    </h2>
  </div>
  <section class="bg-[#E8EDFF] rounded-3xl pb-10 lg:pb-0">
    <div class="flex flex-col lg:flex-row lg:relative lg:h-150">
      <div class="md:w-1/2 p-5 lg:p-30 font-medium space-y-10">
        <div class="pr-10 md:pr-0">
          <h2
            class="text-3xl lg:text-6xl text-gray-800 md:text-4xl tracking-[-1%] leading-10.5 lg:leading-12 font-medium"
          >
            Get ready to scale with our payment APIs
          </h2>
        </div>
        <div class="space-y-10 text-lg lg:text-3xl">
          <div class="flex items-start">
            <div class="shrink-0">
              <img src={GearIcon} alt="Gear Icon" />
            </div>
            <div class="ml-4">
              <h3 class="text-gray-800">Quick setup, easy integration</h3>
            </div>
          </div>
          <div class="flex items-start">
            <div class="shrink-0">
              <img src={CodeBrackets} alt="Gear Icon" />
            </div>
            <div class="ml-4">
              <h3 class="text-gray-800">
                Flexible APIs for any payment use case
              </h3>
            </div>
          </div>
          <div class="flex items-start">
            <div class="shrink-0">
              <img src={StopWatch} alt="Gear Icon" />
            </div>
            <div class="ml-4">
              <h3 class="text-gray-800">
                Production-ready in under 30 minutes
              </h3>
            </div>
          </div>
        </div>
        <div class="mt-8">
          <Button text="Get Started" icon="lucide:arrow-right" swap={true} />
        </div>
      </div>
      <div
        class="p-2 md:p-10 lg:p-0 lg:absolute lg:right-0 lg:transform lg:-translate-y-[10%]"
      >
        <CodeComponeent />
      </div>
    </div>
  </section>
</div>
