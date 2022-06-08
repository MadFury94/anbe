<script setup lang="ts">
import { RouterLink, RouterView } from "vue-router";
import HeaderLayout from "./layouts/headerLayout.vue";
import FooterLayout from "./layouts/footerLayout.vue";
</script>

<template>
  <HeaderLayout />

  <div class="">
    <RouterView />
  </div>

  <FooterLayout />
</template>

<style>
#app {
  background-color: white;
}
</style>
