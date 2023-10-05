<template>
  <div id="foods" class="my-12"></div>
  <div
    class="card-conatiner grid xl:grid-cols-4 md:grid-cols-2 xs:grid-cols-1 gap-4 font-karma text-center"
  >
    <div
      class="card overflow-hidden px-4 xl:h-[620px] mb-4"
      v-for="(item, i) in foods"
      :key="i"
    >
      <div class="card-body">
        <div class="card-img">
          <img :src="item.img" class="mb-4" />
        </div>
        <h2 class="card-text text-2xl dark:text-white">
          {{ item.title }}
        </h2>
        <p class="card-text text-base my-2 dark:text-white">
          {{ item.text }}
        </p>
      </div>
    </div>
  </div>
</template>
<script setup>
import { ref } from "vue";
import imgOne from "../assets/imgs/1.jpg";
import imgTwo from "../assets/imgs/2.jpg";
import imgThree from "../assets/imgs/3.jpg";
import imgFour from "../assets/imgs/4.jpg";
import imgFive from "../assets/imgs/5.jpg";
import imgSix from "../assets/imgs/6.jpg";
import imgSeven from "../assets/imgs/7.jpg";

const foods = ref([
  {
    img: imgOne,
    title: "The Perfect Sandwich, A Real NYC Classic",
    text: "Just some random text, lorem ipsum text praesent tincidunt ipsum lipsum.",
  },
  {
    img: imgTwo,
    title: "Let Me Tell You About This Steak",
    text: "Once again, some random text to lorem lorem lorem lorem ipsum text praesent tincidunt ipsum lipsum.",
  },
  {
    img: imgThree,
    title: "TCherries, interrupted",
    text: "Lorem ipsum text praesent tincidunt ipsum lipsum. What else? ",
  },
  {
    img: imgFour,
    title: "Once Again, Robust Wine and Vegetable Pasta",
    text: "Lorem ipsum text praesent tincidunt ipsum lipsum.",
  },
  {
    img: imgFive,
    title: "All I Need Is a Popsicle",
    text: "Lorem ipsum text praesent tincidunt ipsum lipsum.",
  },
  {
    img: imgSix,
    title: "Salmon For Your Skin",
    text: "Salmon For Your Skin",
  },
  {
    img: imgSeven,
    title: "The Perfect Sandwich, A Real NYC Classic",
    text: "Just some random text, lorem ipsum text praesent tincidunt ipsum lipsum.",
  },
  {
    img: imgOne,
    title: "Le French",
    text: "Lorem lorem lorem lorem ipsum text praesent tincidunt ipsum lipsum.",
  },
]);
</script>
