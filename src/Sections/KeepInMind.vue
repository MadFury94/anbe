<template>
  <div class="bg-gray-800 p-10 child">
    <h1 class="font-bold text-white text-3xl">Keep in mind</h1>
  </div>

  <div
    class="bg-gray-800 grid grid-cols-2 md:grid-cols-4 gap-10 py-10 child px-8"
  >
    <div v-for="(item, index) in About">
      <div
        :class="item.background"
        class="py-20 text-white text-center px-10 rounded-md"
      >
        <h1 class="font-bold text-2xl">{{ item.stats }}</h1>
        <p>{{ item.title }}</p>
      </div>
    </div>

    <!--   <div class="bg-blue-500 text-orange-500 text-center">
      165 completed Projects
    </div>
    <div class="bg-green-500 text-orange-500 text-center">
      3 Office Locations
    </div>
    <div class="bg-white-500 text-orange-500 text-center">CLICK HERE</div>
   -->
  </div>
</template>
<script setup>
const About = [
  {
    title: "Happy Clients",
    background: "bg-orange-500",
    stats: 23,
  },
  {
    title: " Completed Projects",
    background: "bg-green-500",
    stats: 65,
  },

  {
    title: " Office Locations",
    background: "bg-blue-500",
    stats: 13,
  },
  {
    title: " Completed Projects",
    background: "bg-gray-500",
    stats: 20,
  },
];
</script>
