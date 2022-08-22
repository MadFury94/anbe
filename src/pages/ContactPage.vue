<script setup>
import { companyInformation } from "../store/store";
import MiniJumbotron from "../components/MiniJumbotron.vue";
import ContactJumbotron from "../components/icons/ContactJumbotron.vue";
import BladeDivider from "../components/BladeDivider.vue";
import ContactOptions from "../Sections/ContactOptions.vue";
import ContactArea from "../layouts/ContactArea.vue";

const contactTitle = {
  title: "Contact Us",
  // src: "\images\anbe-contact.jpg",
};
// const contactTitle2 = {
//   title2: "Get in Touch",
// };
// const contactText1 = {
//   text: "Or Request a Quote",
// };
const contactJumboData = {
  title: "Get in Touch <br />Or Request a Quote",
  minitext:
    "Our Fabrication facility is located Omueke village, Igwuruta Rd Ikwerre LGA Rivers State. These are our other locations",
};
</script>

<template>
  <div class="relative">
    <img class="absolute z-10 -mt-1 -ml-1" src="/images/svg/blade-curve.svg" />

    <MiniJumbotron
      image="\images\anbe-contact.jpg"
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
  <div class="relative">
    <img class="absolute z-10 -mt-1 -ml-1" src="/images/svg/blade-curve.svg" />
  </div>
  <ContactJumbotron
    title-class="text-5xl text-orange-500 font-bold font-bree"
    :title="contactJumboData.title"
    minitext-class="font-bree"
    :minitext="contactJumboData.minitext"
  />
  <p class="p font-bree"></p>
  <ContactOptions />
  <ContactArea />

  <section class="grid grid-cols-3 py-20">
    <div></div>
    <div class="mapouter">
      <div class="gmap_canvas">
        <iframe
          width="1080"
          height="546"
          id="gmap_canvas"
          src="https://maps.google.com/maps?q=%20Plot%20101%20East%20west%20Road,%20Rumuodara,%20Port%20Harcourt%20Rivers%20State&t=&z=13&ie=UTF8&iwloc=&output=embed"
          frameborder="0"
          scrolling="no"
          marginheight="0"
          marginwidth="0"
        ></iframe
        ><a href="https://www.whatismyip-address.com/divi-discount/"
          >divi discount</a
        ><br /><a href="https://www.embedgooglemap.net"
          >how to add google map in wordpress</a
        >
      </div>
    </div>
    <div></div>
  </section>

  <BladeDivider />
</template>

<style>
.mapouter {
  position: relative;
  text-align: right;
  height: 500px;
  width: 800px;
}

.gmap_canvas {
  overflow: hidden;
  background: none !important;
  height: 500px;
  width: 800px;
}
</style>
