<template>
  <div class="relative">
    <div class="absolute inset-x-0 bottom-0 h-1/2 bg-gray-100" />
    <div class="mx-auto">
      <div class="relative shadow-xl sm:overflow-hidden">
        <div class="absolute inset-0">
          <img
            class="h-full w-full object-cover"
            src="/images/sketch.jpeg"
            alt="People working on laptops"
          />
        </div>
        <div class="relative px-4 py-16 sm:px-6 sm:py-24 lg:py-32 lg:px-8">
          <div class="gap-y-10 gap-x-4 bg-white p-20 lg:grid lg:grid-cols-2">
            <div v-for="(item, index) in 5" :key="index">
              <img
                class="rounded-md"
                src="/images/projects/10306556362782-1.jpg"
              />
              <div class="mt-4 space-y-2">
                <h3>SPDC/NEWCROSS /EROTON/SEPL AT</h3>
                <p>Design/Fabrication/Installation Of Flare Line/Stacks</p>
                <h3>2005 TILL DATE</h3>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
