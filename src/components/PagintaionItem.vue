<template>
  <li
    class="px-4 py-2 bg-white text-black dark:bg-slate-800 dark:text-white hover:bg-black hover:text-white cursor-pointer active:bg-black active:text-white"
  >
    {{ text }}
  </li>
</template>
<script setup>
const props = defineProps({
  text: {
    type: Number,
  },
});
</script>
