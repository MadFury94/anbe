<script setup>
import { ref } from "vue";
import ButtonCommon from "../components/ButtonCommon.vue";

const formData = ref({
  name: "",
  email: "",
  message: "",
});
</script>

<template>
  <div>
    <div class="grid lg:grid-cols-2">
      <div class="-mb-10 bg-orange-500 p-4">
        {{ formData }}

        <h1 class="font-bree text-2xl uppercase lg:text-5xl">Contact Us</h1>
        <hr class="w-20 border-4 border-white" />

        <!-- contact form -->

        <div class="grid-cols-1 gap-x-10 md:grid md:grid-cols-2 lg:p-20">
          <div class="w-full">
            <label
              for="fullname"
              class="block text-sm font-medium text-gray-700"
              >Full name:</label
            >
            <div class="mt-1">
              <input
                v-model="formData.name"
                type="text"
                name="name"
                class="block w-full border-gray-300 py-4 shadow-sm focus:border-orange-500 focus:ring-orange-500 sm:text-sm"
                placeholder="your full name"
              />
            </div>
          </div>
          <div class="w-full">
            <label
              for="fullname"
              class="block text-sm font-medium text-gray-700"
              >Email:</label
            >
            <div class="mt-1">
              <input
                v-model="formData.email"
                type="email"
                name="email"
                class="block w-full border-gray-300 py-4 shadow-sm focus:border-orange-500 focus:ring-orange-500 sm:text-sm"
                placeholder="you@example.com"
              />
            </div>
          </div>
          <div class="col-span-2 w-full">
            <label
              for="fullname"
              class="block text-sm font-medium text-gray-700"
              >Email:</label
            >
            <div class="mt-1">
              <textarea
                v-model="formData.message"
                type="text"
                :rows="10"
                class="block w-full border-gray-300 py-4 shadow-sm focus:border-orange-500 focus:ring-orange-500 sm:text-sm"
                placeholder="please leave us a message"
              />
              <ButtonCommon title="hh" />
            </div>
          </div>
        </div>

        <!-- contact form -->
      </div>
      <div class="bg-gray-200">
        <div class="bg-gray-800">
          <ul class="flex justify-center gap-x-10 py-10 text-2xl text-white">
            <li><i class="fa-brands fa-twitter"></i></li>
            <li><i class="fa-brands fa-linkedin"></i></li>
            <li><i class="fa-brands fa-facebook"></i></li>
          </ul>
        </div>
        <div class="p-20">
          <ul class="space-y-10 font-lato text-lg">
            <li>
              <i class="fa-solid fa-map-location-dot"></i>
              Plot 101 (lakeside Mall), East West Road , Rumuodara, Port
              Harcourt
            </li>
            <li><i class="fa-solid fa-phone"></i>+234 8033 100 539</li>
            <li><i class="fa-solid fa-envelope"></i>anbenig@yahoo.com</li>
          </ul>
        </div>
      </div>
    </div>
  </div>
</template>
