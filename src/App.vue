<script setup>
import NavBar from "./components/NavBar.vue";
import CardView from "./components/CardView.vue";
import PaginationComp from "./components/paginationcomp.vue";
import AboutPage from "./components/AboutPage.vue";
import FooterComp from "./components/FooterComp.vue";
</script>

<template>
  <div class="md:container mx-auto xl:px-32 px-12">
    <NavBar />
    <CardView />
    <PaginationComp pageCount="4" />
    <hr
      class="h-[1px] xl:my-24 m-14 text-slate-900 bg-slate-800 rounded-full border-none"
    />
    <AboutPage />
    <hr
      class="h-[1px] xl:my-24 m-14 text-slate-900 bg-slate-800 rounded-full border-none"
    />
    <FooterComp />
  </div>
</template>
