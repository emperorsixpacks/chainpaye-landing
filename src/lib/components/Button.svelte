<script lang="ts">
  import Icon from "@iconify/svelte";

  const { text, url = "#", icon = "", swap = false } = $props();
</script>

<button class="bg-blue-700 text-white py-3 px-6 rounded-lg cursor-pointer">
  <span class="flex items-center gap-2 font-bold" class:flex-row-reverse={swap}
    ><Icon {icon} width="20" height="20" />{text}
  </span>
</button>
