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
import MiniJumbotron from "../components/MiniJumbotron.vue";
import Localcontent from "../Sections/localcontent.vue";
import BladeDivider from "../components/BladeDivider.vue";
import Ourleader from "../Sections/ourleader.vue";
import Background_writeup from "../Sections/background_writeup.vue";

const aboutData = {
  title: "About Us",
  text: `ANBE NIGERIA LTD has executed various projects in the areas of
                  Design, Fabrication and installation of smokeless flares
                  Onshore/Offshore fabrication works, Procurement and
                  Installation of Remote Ignition System, Repair of corrosion
                  defect by clamping. Leak repair. Flare change out projects
                  Flow line replacement, maintenance and installation, Flow
                  station/facilities upgrade and rehabilitation. Elf Petroleum:
                  Lease of operational vehicles for Port Harcourt, Lagos and
                  Abuja offices. Supply of boats and vehicles to SPDC for
                  National Immunization Programme.`,
  image: "/images/handyman_02.jpeg",
};
const serviceData = {
  title: "About Us",
  text: `We have in our employ experienced and professionally qualified personnel in fabrication and construction field of services. Our fabrication facility is located in Omueke Village Igwuruta Rd Ikwerre L.G.A Rivers State.`,
  image: "/images/handyman_02.jpeg",
};
</script>

<template>
  <div class="relative">
    <img class="absolute z-10 -mt-1 -ml-1" src="/images/svg/blade-curve.svg" />

    <!-- <MiniJumbotron
      :image="aboutData.image"
      text-class="text-white lg:w-[800px] leading-8 pt-8"
      :title="aboutData.title"
      title-class="text-5xl text-orange-500 font-bold font-bree"
      :text="aboutData.text"
      padding="sm:py-24 lg:py-32 py-10 "
    /> -->
    <Background_writeup />

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
  <Ourleader />
  <div>
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
  </div>
  <Localcontent />
  <BladeDivider />
</template>
