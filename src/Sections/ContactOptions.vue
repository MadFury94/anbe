<template>
  <div>
    <section class="grid gap-y-10 px-10 py-20 md:grid-cols-2 lg:grid-cols-3">
      <div v-for="(item, index) in serviceList" :key="index">
        <div class="box-border h-48 w-48 items-center gap-x-4 border-4 p-4">
          <!-- <img
            :src="`images/icons/${item.icon}`"
            alt="supply icon"
            class="w-16"
          /> -->
          <h1 class="text-center font-bree text-sm font-bold uppercase">
            {{ item.title }}
          </h1>
          <p class="text-center font-bree text-sm font-light">
            {{ item.subtitle }}
          </p>
        </div>
      </div>
    </section>
  </div>
</template>
<script setup>
const serviceList = [
  {
    // icon: "construction-icon-7-gray.png",

    title: "Our Administrative Office",
    subtitle: "Road B, House 106, Oba Adeyanka Oyekan Estate, Lekki Phase 1",
  },
  {
    // icon: "construction-icon-5-gray.png",

    title: "Branch Office",
    subtitle:
      "LAKESIDE MALL Plot 101 East West Road, Rumudara, Port Harcourt Rivers State",
  },
  {
    // icon: "construction-icon-2-gray.png",

    title: "Branch office",
    subtitle: "11 MCC Road, Off Ernheren Road, Warri Delta State",
  },
];
</script>
