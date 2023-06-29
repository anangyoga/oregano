<script setup>
const activeMenu = "Home";
const menus = ["Home", "Delivery", "Pricing", "FAQs", "Contact"];
import HamburgerIcon from "../assets/hamburger.svg";
</script>

<template>
  <nav class="flex items-center justify-between px-6 py-8 sm:px-24 sm:py-8 max-w-screen-xl mx-auto">
    <a href="#" class="text-4xl font-bold tracking-wide">Oregan<span class="text-green">o</span></a>

    <div class="hidden md:flex md:items-center md:space-x-14">
      <ul class="flex items-center space-x-8">
        <li class="text-xl font-medium group" :class="{ 'text-green': activeMenu === menu }" v-for="menu in menus">
          <a href="#"> {{ menu }} </a>
          <div class="h-0.5 bg-green scale-x-0 group-hover:scale-100 transition-transform origin-left rounded-full duration-300 ease-out"></div>
        </li>
      </ul>

      <button class="flex items-center justify-center h-13 bg-green px-7 font-medium text-white rounded-xl hover:shadow-primary transition-shadow duration-300">Get Started</button>
    </div>
    <button class="block md:hidden">
      <HamburgerIcon class="w-8 h-8 fill-current text-gray-900" />
    </button>
  </nav>
</template>
