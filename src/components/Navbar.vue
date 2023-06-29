<script setup>
const activeMenu = "Home";
const menus = ["Home", "Delivery", "Pricing", "FAQs", "Contact"];
</script>

<template>
  <nav class="flex items-center justify-between px-24 py-8 max-w-screen-xl mx-auto">
    <a href="#" class="text-4xl font-bold tracking-wide">Oregan<span class="text-green">o</span></a>

    <ul class="flex items-center space-x-8">
      <li class="text-xl font-medium" :class="{ 'text-green': activeMenu === menu }" v-for="menu in menus">
        <a href="#"> {{ menu }} </a>
      </li>
    </ul>
  </nav>
</template>
