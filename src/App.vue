<script setup lang="ts">
import { RouterView } from "vue-router";
import HeaderLayout from "./layouts/headerLayout.vue";

import FooterLayout from "./layouts/FooterLayout.vue";
</script>

<template>
  <HeaderLayout />

  <div class="">
    <RouterView />
  </div>

  <FooterLayout></FooterLayout>
</template>

<style>
#app {
  background-color: white;
}
</style>
