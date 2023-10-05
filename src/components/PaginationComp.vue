<template>
  <div id="pagination">
    <div class="mx-auto">
      <ul class="pagination flex justify-center mx-auto w-fit dark:rounded">
        <!--Previous Button-->

        <li
          class="flex items-center px-2 py-2 dark:bg-slate-800 dark:text-white bg-white text-black hover:bg-black hover:text-white cursor-pointer rounded-l-lg"
        >
          <svg
            xmlns="http://www.w3.org/2000/svg"
            width="20"
            height="20"
            viewBox="0 0 24 24"
          >
            <path
              fill="currentColor"
              fill-rule="evenodd"
              d="M17.488 4.43a.75.75 0 0 1 .081 1.058L11.988 12l5.581 6.512a.75.75 0 1 1-1.139.976l-6-7a.75.75 0 0 1 0-.976l6-7a.75.75 0 0 1 1.058-.081Zm-4 0a.75.75 0 0 1 .081 1.058L7.988 12l5.581 6.512a.75.75 0 1 1-1.138.976l-6-7a.75.75 0 0 1 0-.976l6-7a.75.75 0 0 1 1.057-.081Z"
              clip-rule="evenodd"
            />
          </svg>
        </li>

        <PagintaionItem
          v-for="number in Number(pageCount)"
          :key="number"
          :text="number"
        />

        <!--Next Button-->
        <li
          class="flex items-center px-2 py-1 dark:bg-slate-800 dark:text-white bg-white text-black hover:bg-black hover:text-white cursor-pointer rounded-r-lg"
        >
          <svg
            xmlns="http://www.w3.org/2000/svg"
            width="20"
            height="20"
            viewBox="0 0 24 24"
          >
            <path
              fill="currentColor"
              fill-rule="evenodd"
              d="M6.512 4.43a.75.75 0 0 1 1.057.082l6 7a.75.75 0 0 1 0 .976l-6 7a.75.75 0 0 1-1.138-.976L12.012 12L6.431 5.488a.75.75 0 0 1 .08-1.057Zm4 0a.75.75 0 0 1 1.058.082l6 7a.75.75 0 0 1 0 .976l-6 7a.75.75 0 0 1-1.14-.976L16.013 12l-5.581-6.512a.75.75 0 0 1 .081-1.057Z"
              clip-rule="evenodd"
            />
          </svg>
        </li>
      </ul>
    </div>
  </div>
</template>

<script setup>
import PagintaionItem from "./PagintaionItem.vue";
const props = defineProps({
  pageCount: {
    type: Number,
    default: 1,
  },
});
</script>
