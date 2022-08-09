<script setup>
import ListOfServices from "../Sections/ListOfServices.vue";
import OrangeBackground from "../Sections/OrangeBackground.vue";
import CoreAreas from "../Sections/CoreAreas.vue";
import logo_area from "../Sections/logo_area.vue";
import contact_us from "../Sections/contact_us.vue";
import JumboTronComponent from "../components/JumboTronComponent.vue";
// import JumboTron from "../layouts/JumboTron.vue";
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
    <ListOfServices />
    <OrangeBackground />
    <!-- core areas -->
    <JumboTronComponent
      :hasTitle="false"
      title=" ANBE NIG"
      subTitle=" We’ve Been Building For Over 20 years"
      text="Among the non technical staff are Clerks, Administrative Officers, Accountant, Office Managers and Marketing officers."
      link-title="VIEW OUR WORK"
      image="/images/gas-flare.jpeg"
      page-link="project"
    />
    <!-- core areas -->

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
