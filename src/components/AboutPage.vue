<template>
  <div id="about ">
    <h3 class="text-center text-3xl text-black dark:text-slate-100">
      About Me, The Food Man
    </h3>
    <div class="about-img flex justify-center my-5 mt-10">
      <img :src="Chef" />
    </div>
    <div class="description text-center dark:text-slate-100">
      <h2 class="text-2xl my-5 mt-10 font-bold">I am Who I Am!</h2>
      <p class="italic dark:text-slate-100">With Passion For Real, Good Food</p>
      <p class="px-4 text-base my-5">
        Just me, myself and I, exploring the universe of unknownment. I have a
        heart of love and an interest of lorem ipsum and mauris neque quam blog.
        I want to share my world with you. Praesent tincidunt sed tellus ut
        rutrum. Sed vitae justo condimentum, porta lectus vitae, ultricies
        congue gravida diam non fringilla. Praesent tincidunt sed tellus ut
        rutrum. Sed vitae justo condimentum, porta lectus vitae, ultricies
        congue gravida diam non fringilla.
      </p>
    </div>
  </div>
</template>
<script setup>
import Chef from "../assets/imgs/chef.jpg";
</script>
