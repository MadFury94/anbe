<script setup>
import BackgroundImage from "../Sections/BackgroundImage.vue";
import List_of_services from "../Sections/list_of_services.vue";
import orange_background from "../Sections/orange_background.vue";
import core_areas from "../Sections/core_areas.vue";
import logo_area from "../Sections/logo_area.vue";
import contact_us from "../Sections/contact_us.vue";
import JumboTronComponent from "../components/JumboTronComponent.vue";
// import JumboTron from "../layouts/JumboTron.vue";

const JumboTron = {
  title: "",
  text: `  “We aim to become an international Pipeline, Engineering and
            Construction service company that provides services of International
            standard”`,
};
</script>

<template>
  <main>
    <JumboTronComponent
      title=" ANBE NIG"
      text="“We aim to become an international Pipeline, Engineering and
            Construction service company that provides services of International
            standard”"
      link-title="VIEW OUR WORK"
      image="/images/construction-35.jpeg"
      page-link="project"
    />
    <List_of_services></List_of_services>
    <orange_background></orange_background>
    <core_areas></core_areas>
    <logo_area></logo_area>
    <contact_us></contact_us>

    <!-- // background section   background image  -->
    <!-- //   list of services  -->
    <!-- //   orange background with write up  -->
    <!-- //   core areas  -->
    <!-- //   button  -->
  </main>
</template>

<style scoped>
#bg-image {
  background-color: #cccccc;
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  position: relative;
}
</style>
