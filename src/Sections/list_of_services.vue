<template>
  <div>
    <section class="grid md:grid-cols-2 lg:grid-cols-3 gap-10 p-20">
      <div v-for="(item, index) in serviceList" :key="index">
        <div class="flex gap-x-4 items-center">
          <img
            :src="`images/icons/${item.icon}`"
            alt="supply icon"
            class="w-16"
          />
          <p class="uppercase">
            {{ item.title }}
          </p>
        </div>
      </div>
    </section>
  </div>
</template>
<script setup>
const serviceList = [
  {
    icon: "construction-icon-7-gray.png",

    title: "Supply of boats and vehicles to SPDC for Immunization Programme",
  },
  {
    icon: "construction-icon-5-gray.png",

    title: "Design, Fabrication and installation of smokeless flares",
  },
  {
    icon: "construction-icon-2-gray.png",

    title: "Procurement and Installation of Remote Ignition System",
  },
  {
    icon: "construction-icon-1-gray.png",

    title:
      "Our fabrication facility is located in Omueke Village Igwuruta Rd Ikwerre L.G.A Rivers State",
  },
  {
    icon: "construction-icon-6-gray.png",

    title: "Flow line replacement, maintenance and installation",
  },
  {
    icon: "construction-icon-4-gray.png",

    title: "Flow station/facilities upgrade and rehabilitation",
  },
];
</script>
