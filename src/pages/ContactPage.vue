<script setup>
import { companyInformation } from "../store/store";
import MiniJumbotron from "../components/MiniJumbotron.vue";
import ContactJumbotron from "../components/icons/ContactJumbotron.vue";
import BladeDivider from "../components/BladeDivider.vue";
import ContactOptions from "../Sections/ContactOptions.vue";
import ContactArea from "../layouts/ContactArea.vue";

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

    <MiniJumbotron
      image="https://anbenig.com/wp-content/uploads/2019/12/handyman_01.jpg"
      title-class="text-5xl text-orange-500 font-bold font-bree"
      :title="contactTitle.title"
      :text="null"
    />

    <div class="">
      <div class="grid-cols-4 items-center font-bree text-2xl lg:grid">
        <div></div>
        <div class="bg-orange-500 py-10 px-20 text-white">Get A Quote</div>
        <div class="col-span-2 px-20 py-10 text-gray-500">
          CALL US:
          <span class="text-orange-500">{{
            companyInformation.contactNumbers.phone1
          }}</span>
        </div>
      </div>
    </div>
  </div>
  <ContactJumbotron
    title-class="text-5xl text-orange-500 font-bold font-bree"
    :title="contactTitle2.title2"
    text-class="text-5xl text-orange-500 font-bold font-bree"
    :text="contactText1.text"
    minitext="Our Fabrication facility is located Omueke village, Igwuruta Rd Ikwerre LGA
    Rivers State. These are our other locations"
  />
  <p class="p font-bree"></p>
  <ContactOptions />
  <ContactArea />
  <BladeDivider />
</template>
