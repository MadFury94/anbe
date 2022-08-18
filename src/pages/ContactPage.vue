<script setup>
import MiniJumbotron from "../components/MiniJumbotron.vue";
import ContactJumbotron from "../components/icons/ContactJumbotron.vue";
import BladeDivider from "../components/BladeDivider.vue";

const contactTitle = {
  title: "Contact Us",
  image: "https://anbenig.com/wp-content/uploads/2019/12/handyman_01.jpg",
};
const contactTitle2 = {
  title2: "Get in Touch",
};
const contactText1 = {
  text: "Or Request a Quote",
};
</script>

<template>
  <div class="relative">
    <img class="absolute z-10 -mt-1 -ml-1" src="/images/svg/blade-curve.svg" />
  </div>

  <MiniJumbotron
    image="https://anbenig.com/wp-content/uploads/2019/12/handyman_01.jpg"
    title-class="text-5xl text-orange-500 font-bold font-bree"
    :title="contactTitle.title"
    :text="null"
  />
  <ContactJumbotron
    title-class="text-5xl text-orange-500 font-bold font-bree"
    :title="contactTitle2.title2"
    text-class="text-5xl text-orange-500 font-bold font-bree"
    :text="contactText1.text"
  />
  <p class="font-bree">
    Our Fabrication facility is located Omueke village, Igwuruta Rd Ikwerre LGA
    Rivers State. These are our other locations
  </p>
  <BladeDivider />
</template>
