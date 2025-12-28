<script lang="ts">
  import Icon from "@iconify/svelte";

  const { text, url = "#", icon = "", swap = false, newTab = true } = $props();
</script>

<a
  href={url}
  class="inline-block bg-blue-700 text-white py-3 px-6 rounded-lg cursor-pointer"
  target={newTab ? "_blank" : "_self"}
  rel={newTab ? "noopener noreferrer" : undefined}
>
  <span class="flex items-center gap-2 font-bold" class:flex-row-reverse={swap}>
    {#if icon}
      <Icon {icon} width="20" height="20" />
    {/if}
    {text}
  </span>
</a>
