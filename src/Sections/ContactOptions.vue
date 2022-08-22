<template>
  <div>
    <section
      class="grid place-content-center gap-y-10 gap-x-20 px-10 py-20 sm:grid-cols-3 lg:grid-cols-3"
    >
      <div v-for="(item, index) in serviceList" :key="index">
        <div
          class="box-border h-40 items-center gap-x-4 rounded-md border-4 border-gray-200 p-10"
        >
          <!-- <img
            :src="`images/icons/${item.icon}`"
            alt="supply icon"
            class="w-16"
          /> -->
          <h1 class="text-center font-bree text-sm font-bold uppercase">
            {{ item.title }}
          </h1>
          <p class="text-center font-bree text-sm font-light leading-7">
            {{ item.subtitle }}
          </p>
        </div>
      </div>
    </section>
  </div>
</template>
<script setup>
import { companyInformation } from "../store/store";

const serviceList = [
  {
    // icon: "construction-icon-7-gray.png",

    title: "Our Administrative Office",
    subtitle: ` ${companyInformation.value.addresses.address1}`,
  },
  {
    // icon: "construction-icon-5-gray.png",

    title: "Branch Office",
    subtitle: ` ${companyInformation.value.addresses.address2}`,
  },
  {
    // icon: "construction-icon-2-gray.png",

    title: "Branch office",
    subtitle: `${companyInformation.value.addresses.address3}`,
  },
];
</script>
