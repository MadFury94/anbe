<!-- <script setup>
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
</template> -->
<script setup>
import { companyInformation } from "../store/store";
import Localcontent from "../Sections/localcontent.vue";
import BladeDivider from "../components/BladeDivider.vue";
import Ourleader from "../Sections/ourleader.vue";
import Background_writeup from "../Sections/background_writeup.vue";
</script>

<template>
  <div class="relative">
    <img class="absolute z-10 -mt-1 -ml-1" src="/images/svg/blade-curve.svg" />

    <Background_writeup />
  </div>
  <div><img class="-mt-2" src="/images/svg/blade.svg" /></div>
  <Ourleader />
  <div class="py-10">
    <div
      class="grid-cols-4 items-center text-justify font-bree text-2xl lg:grid"
    >
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
  <!-- <div>
    <MiniJumbotron
      text-class="text-white w-[800px] leading-8 pt-8"
      title="Related Services"
      title-class="text-5xl text-orange-500 font-bold font-bree"
      :text="serviceData.text"
      padding="py-10"
      image=""
      image-color="bg-white"
      textClass="text-gray-500"
    />
  </div> -->
  <Localcontent />
  <BladeDivider />
</template>
