<!-- <template>
  <div class="flex justify-between p-2 bg-blue-500 text-white">
    <div>
      <img
        alt="Vue logo"
        class="h-10"
        src="https://anbenig.com/wp-content/uploads/2017/09/logo-01.png"
        width="125"
        height="125"
      />
    </div>
    <div>
      <nav class="flex gap-10">
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/about">About</RouterLink>
        <RouterLink to="/about">Services</RouterLink>
        <RouterLink to="/about">Contact</RouterLink>
        <RouterLink to="/about">supports them</RouterLink>
      </nav>
    </div>
  </div>
</template> -->
<template>
  <header class="text-black-100 bg-white text-lg font-semibold">
    <div class="flex items-center justify-between">
      <div>
        <a href="https://anbenig.com" target="_blank">
          <img
            class="w-20"
            src="https://anbenig.com/wp-content/uploads/2017/09/logo-01.png"
            alt="anbe logo"
          />
        </a>
      </div>
      <nav class="hidden md:block">
        <ul class="flex gap-x-4">
          <RouterLink to="/">Home</RouterLink>

          <RouterLink to="/about">About Anbe</RouterLink>

          <RouterLink to="/about">Services</RouterLink>

          <RouterLink to="/about">Contact</RouterLink>
        </ul>
      </nav>
      <button class="md:hidden">menu</button>
    </div>
  </header>
</template>
