<script setup>
import Background_writeup from "../Sections/background_writeup.vue";
import Backgroundimage_button from "../Sections/backgroundimage_button.vue";
import Localcontent from "../Sections/localcontent.vue";
import Ourleader from "../Sections/ourleader.vue";
</script>

<template>
  <main class="relative">
    <img class="absolute z-10 -mt-1 -ml-1" src="/images/svg/blade-curve.svg" />

    <Background_writeup />

    <Backgroundimage_button></Backgroundimage_button>
    <Ourleader></Ourleader>
    <Localcontent></Localcontent>
  </main>
</template>
