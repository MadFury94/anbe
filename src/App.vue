<script setup lang="ts">
import { RouterView } from "vue-router";
import HeaderLayout from "./layouts/headerLayout.vue";

import FooterLayout from "./layouts/footerLayout.vue";
</script>

<template>
  <HeaderLayout />

  <div class="w-screen">
    <RouterView />
  </div>

  <FooterLayout></FooterLayout>
</template>

<style>
#app {
  background-color: white;
}
</style>
