<template>
  <main class="grid grid-cols-3">
    <section class="bg-orange-500 py-20 px-4">
      <div class="space-y-10 px-10">
        <div class="">
          <div v-for="(item, index) in aboutUs" :key="index">
            <div class="flex items-center space-x-6 py-4">
              <div>
                <i class="fa-solid fa-angles-right text-2xl text-white"></i>
              </div>
              <div class="font-lato text-lg leading-7 text-slate-700">
                {{ item.text }}
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
    <section class="col-span-2">
      <div class="space-y-8 bg-gray-100 p-28">
        <div>
          <h1 class="font-bree text-5xl font-bold">Core</h1>
          <!-- divider -->
          <hr class="my-10 w-20 border-4 border-orange-500" />
        </div>
        <section class="grid grid-cols-2 gap-x-10 text-justify leading-7">
          <div>
            Our main function remains Pipeline Construction, Installation/Repair
            of Pipeline, Design and Fabrication of Smokeless Flare stacks and
            Remote Ignition Systems, Stock Pilling, Procurement, Construction
            and Fabrication Engineering design for Oil and Gas facilities, ANBE
            Technical Partners provide expertise technical support needed in
            carrying out activities within the above scope. This has helped us
            in meeting the requirements of our range of clients.
          </div>
          <div>
            Through our close association with these construction groups, ANBE
            is uniquely equipped to apply the lessons learnt on its projects to
            benefit the needs of its clients. We are committed to estimates of
            budget and schedule which are backed-up with real project data and
            advise as to how further economies can be made on future
            developments. In today’s commercial environment we believe this
            experience is of vital importance to those contemplating similar
            developments
          </div>
        </section>
      </div>
      <section class="flex items-center justify-between bg-gray-800 p-8 py-4">
        <h1 class="font-serif text-2xl text-white">
          Request a call from representative
        </h1>
        <div class="p-10 px-44">
          <ButtonCommon title="  ASK FOR CALL" />
        </div>
      </section>
    </section>
  </main>
</template>
<script setup>
import { ref } from "vue";
import ButtonCommon from "../components/ButtonCommon.vue";

const aboutUs = ref([
  {
    text: "Our quality control system is formerly documented to meet requirements of BS EN 9000 and it is geared towards continuing performance improvements.",
  },
  {
    text: "Our quality control .",
  },
  {
    text: "Our quality control system is formerly documented to meet requirements of BS EN 9000 and it is geared towards continuing performance improvements.",
  },
]);
</script>
