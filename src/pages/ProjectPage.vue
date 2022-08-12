<script setup>
import JumboTronComponent from "../components/JumboTronComponent.vue";
import ProjectListComponent from "../components/ProjectListComponent.vue";
</script>

<template>
  <div class="relative">
    <img class="absolute z-10 -mt-1 -ml-1" src="/images/svg/blade-curve.svg" />

    <JumboTronComponent
      class=""
      title-class="text-orange-500"
      :has-button="false"
      text-class="text-lg"
      title=" ANBE NIG"
      text="ANBE NIGERIA LTD has executed various projects in the areas of Design, Fabrication and installation of smokeless flares Onshore/Offshore fabrication works, Procurement and Installation of Remote Ignition System, Repair of corrosion defect by clamping. Leak repair. Flare change out projects Flow line replacement, maintenance and installation, Flow station/facilities upgrade and rehabilitation. Elf Petroleum: Lease of operational vehicles for Port Harcourt, Lagos and Abuja offices. Supply of boats and vehicles to SPDC for National Immunization Programme."
      link-title="VIEW OUR WORK"
      image="/images/Smoking-Flare.png"
      page-link="project"
    />
    <div class="">
      <div class="grid-cols-4 items-center font-bree text-2xl lg:grid">
        <div></div>
        <div class="bg-orange-500 py-10 px-20 text-white">Get A Quote</div>
        <div class="col-span-2 px-20 py-10 text-gray-500">
          CALL US: <span class="text-orange-500">+2348033100539</span>
        </div>
      </div>
    </div>
  </div>
  <ProjectListComponent />
</template>
