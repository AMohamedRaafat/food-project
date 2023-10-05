<template>
  <div
    id="nav"
    class="flex justify-between py-4 font-karma sticky top-0 bg-white dark:bg-slate-950"
  >
    <div class="navbar">
      <span
        class="ic:round-menu cursor-pointer dark:text-white"
        @click="toggleShow"
        ><svg
          xmlns="http://www.w3.org/2000/svg"
          width="32"
          height="32"
          viewBox="0 0 24 24"
        >
          <path
            fill="currentColor"
            fill-rule="evenodd"
            d="M20.75 7a.75.75 0 0 1-.75.75H4a.75.75 0 0 1 0-1.5h16a.75.75 0 0 1 .75.75Zm0 5a.75.75 0 0 1-.75.75H4a.75.75 0 0 1 0-1.5h16a.75.75 0 0 1 .75.75Zm0 5a.75.75 0 0 1-.75.75H4a.75.75 0 0 1 0-1.5h16a.75.75 0 0 1 .75.75Z"
            clip-rule="evenodd"
          /></svg
      ></span>
    </div>
    <div>
      <span class="text-2xl dark:text-white">My Food</span>
    </div>
    <div>
      <span class="hidden xl:block text-2xl dark:text-white">Mail</span>
    </div>

    <!--Fixed Nav-->
    <div
      :class="`floating-nav h-screen fixed top-0 transition-all duration-500 shadow-lg shadow-slate-700 bg-white text-black xl:w-[650px] w-[400px]  dark:bg-slate-900 dark:text-white 
        ${show ? 'left-1' : 'left-[-650px]'}
        `"
    >
      <ul class="p-0 font-karma text-3xl text-left">
        <li
          class="hover:bg-gray-400 px-4 py-6 cursor-pointer"
          @click="closeMenu"
        >
          Close Menu
        </li>
        <li class="my-12 hover:bg-gray-400 px-4 py-6 cursor-pointer">Food</li>
        <li class="hover:bg-gray-400 px-4 py-6 cursor-pointer">About</li>
      </ul>
    </div>
  </div>
</template>
<script setup>
import { ref } from "vue";

const show = ref(false);

const toggleShow = () => {
  show.value = !show.value;
};
const closeMenu = () => {
  show.value = false;
};
</script>
