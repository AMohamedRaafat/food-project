<template>
  <div id="footer" class="h-[300px]">
    <div class="grid xl:grid-cols-3 md:grid-cols-2 xs-grid:cols-1">
      <!--Footer-->
      <div class="flex flex-col justify-between px-10 mb-5">
        <div class="title dark:text-white">
          <h2 class="text-3xl uppercase">Footer</h2>
        </div>
        <div class="desc dark:text-white my-8">
          <p class="text-lg">
            Praesent tincidunt sed tellus ut rutrum. Sed vitae justo
            condimentum, porta lectus vitae, ultricies congue gravida diam non
            fringilla.
          </p>
        </div>
        <div class="copy dark:text-white">
          <span>Powered by :</span>
        </div>
      </div>
      <div class="flex flex-col justify-between px-10 mb-5">
        <div class="title dark:text-white">
          <h2 class="text-3xl uppercase">Blog Posts</h2>
        </div>

        <!--Blog Posts-->
        <div class="items">
          <div
            class="flex items-center px-3 py-3 cursor-pointer hover:bg-gray-300"
          >
            <img :src="s" alt="" class="w-14" />
            <div class="ml-5 dark:text-white">
              <p>Lorem</p>
              <p class="mt-2">Sed mattis nunc</p>
            </div>
          </div>
          <div
            class="flex items-center px-3 cursor-pointer hover:bg-gray-300 py-3 mt-5"
          >
            <img :src="a" alt="" class="w-14" />
            <div class="ml-5 dark:text-white">
              <p>Ipsum</p>
              <p class="mt-2">Praes tinci sed</p>
            </div>
          </div>
        </div>
      </div>

      <!--Popular Tags-->

      <div class="flex flex-col px-10 mb-5">
        <div class="title dark:text-white h-20">
          <h2 class="text-3xl uppercase">Populat Tags</h2>
        </div>
        <div class="desc dark:text-white">
          <ul class="flex flex-wrap gap-1 items-center">
            <li
              class="w-fit p-2 my-2 overflow-hidden text-center bg-black text-white dark:bg-white dark:text-black"
            >
              Travel
            </li>
            <li
              class="w-fit px-2 my-2 overflow-hidden text-center bg-slate-700 text-white dark:bg-gray-400 dark:text-black"
            >
              New York
            </li>
            <li
              class="w-fit px-2 my-2 overflow-hidden text-center bg-slate-700 text-white dark:bg-gray-400 dark:text-black"
            >
              Dinner
            </li>
            <li
              class="w-fit px-2 my-2 overflow-hidden text-center bg-slate-700 text-white dark:bg-gray-400 dark:text-black"
            >
              Salmon
            </li>
            <li
              class="w-fit px-2 my-2 overflow-hidden text-center bg-slate-700 text-white dark:bg-gray-400 dark:text-black"
            >
              France
            </li>
            <li
              class="w-fit px-2 my-2 overflow-hidden text-center bg-slate-700 text-white dark:bg-gray-400 dark:text-black"
            >
              Drinks
            </li>
          </ul>
        </div>
      </div>
    </div>
  </div>
</template>
<script setup>
import s from "../assets/imgs/s.jpg";
import a from "../assets/imgs/a.jpg";
</script>
