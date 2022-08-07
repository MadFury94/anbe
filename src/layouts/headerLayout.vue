<template>
  <header class="text-black-100 text-lg font-semibold xl:px-60 hidden lg:block">
    <div class="flex items-center justify-between">
      <div>
        <a href="" target="_blank">
          <img
            class="w-20"
            src="../assets/images/anbe-logo.png"
            alt="anbe logo"
          />
        </a>
      </div>
      <div>
        <nav class="font-bree">
          <div class="flex gap-x-6 px-3">
            <div
              class="flex gap-x-8 px-3"
              v-for="(item, index) in headerRoutes"
              :key="index"
            >
              <RouterLink active-class="active" :to="{ name: item.name }">{{
                item.title
              }}</RouterLink>
            </div>
          </div>
        </nav>
      </div>
    </div>
  </header>

  <!-- mobile menu design -->
  <header class="lg:hidden">
    <div class="flex justify-between items-center px-8">
      <div>
        <a href="#" target="_blank">
          <img
            class="w-20"
            src="../assets/images/anbe-logo.png"
            alt="anbe logo"
          />
        </a>
      </div>
      <div class="relative">
        {{ isMenuOpen }}
        <button @click="toggleMenu" class="bg-orange-400 p-2">Menu</button>
        <div
          class="bg-slate-400 z-10 mt-4 absolute p-10 -ml-5"
          :class="isMenuOpen ? 'block' : 'hidden'"
        >
          <div v-for="(item, index) in headerRoutes" :key="index">
            <RouterLink
              @click="toggleMenu"
              active-class="active"
              :to="{ name: item.name }"
              >{{ item.title }}</RouterLink
            >
          </div>
        </div>
      </div>
    </div>
  </header>
  <!-- mobile menu design -->
</template>

<script setup>
import { ref } from "vue";

const headerRoutes = [
  {
    path: "/",
    name: "home",
    title: "Home",
  },
  {
    path: "/about",
    name: "about",
    title: "About",
  },
  {
    path: "/projects",
    name: "project",
    title: "Projects",
  },
  {
    path: "/services",
    name: "services",
    title: "Services",
  },
  {
    path: "/contact",
    name: "contact",
    title: "Contact",
  },
];

const isMenuOpen = ref(true);

function toggleMenu() {
  isMenuOpen.value = !isMenuOpen.value;
  console.log(isMenuOpen.value, "here");
}
</script>

<style lang="scss" scoped>
.active {
  @apply text-orange-400;
}
</style>
