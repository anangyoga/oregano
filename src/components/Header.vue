<script setup>
import StarIcon from "../assets/star.svg";
import FuelerIcon from "../assets/fueler.svg";
</script>
<template>
  <div class="flex flex-wrap-reverse justify-between gap-y-24 py-12 px-6 sm:px-8 md:px-12 lg:px-16 xl:px-24 max-w-screen-xl mx-auto">
    <div class="relative md:w-1/2 w-full">
      <img class="absolute top-0 right-0 md:-top-4 md:-right-8 w-24 h-auto" src="/img/leaf.png" alt="leaf" />
      <span class="flex items-center px-1 text-xl text-green">
        <span class="font-medium">100% Organic food</span>
        <img class="h-8 w-auto" src="/img/vegetable.png" alt="vegetable" />
      </span>
      <h1 class="pt-4 text-4xl sm:text-5xl lg:text-6xl font-bold tracking-tighter leading-tight">Healthy Lifestyle is your only <span class="text-green whitespace-nowrap">unfair advantage</span></h1>
      <p class="pt-8 sm:text-lg max-w-md font-normal text-gray-600 leading-relaxed">Choose healthy habits with Oregano daily meal prepared by our expert nutritionist and chef.</p>
      <div class="flex space-x-6 pt-8">
        <button class="flex justify-center items-center bg-green text-white font-medium h-13 px-8 rounded-xl hover:shadow-primary transition-shadow duration-300 ease-out">Get Started</button>
        <button class="flex justify-center items-center font-medium h-13 px-8 rounded-xl ring-1 ring-black hover:shadow-2xl transition-shadow duration-300">Explore Menu</button>
      </div>
      <div class="flex pt-20 items-center">
        <img class="w-24 h-auto" src="/img/chef.png" alt="chef" />
        <div class="pt-5 pl-3">
          <h4 class="text-xl font-bold leading-relaxed">Chef of the month</h4>
          <div class="inline-flex text-gray-600 leading-relaxed">People loved his 🍳</div>
          <p class="text-green font-bold leading-relaxed">80+ famous dishes</p>
        </div>
      </div>
    </div>
    <div class="relative flex-1 flex flex-col justify-between">
      <img class="max-w-xl w-80 lg:w-full drop-shadow-2xl self-end" src="/img/dish.png" alt="dish" />
      <div class="absolute right-0 lg:-right-6 top-0 lg:top-28 flex flex-col py-5 px-7 rounded-2xl shadow-xl bg-white/80 backdrop-blur-xl hover:-translate-y-2 hover:shadow-2xl transition-all duration-300">
        <div class="flex -space-x-3">
          <div v-for="i in 3" class="w-13 h-13 rounded-full border-4 border-white object-cover overflow-hidden">
            <img :src="`/public/img/avatar-${i}.jpeg`" alt="" />
          </div>
        </div>
        <h3 class="pt-3 font-bold">Happy Customers</h3>
        <div class="flex items-center gap-x-[1px] leading-relaxed text-gray-600">
          <StarIcon class="w-5 h-5" />
          <p>4.9 (+2.5K Ratings)</p>
        </div>
      </div>
      <div class="absolute left-0 bottom-0 md:bottom-32 lg:bottom-16 flex bg-white/80 rounded-2xl shadow-xl backdrop-blur-xl hover:-translate-y-2 hover:shadow-2xl transition-all duration-300">
        <img class="w-auto h-20 self-end" src="/img/driver.png" alt="driver" />
        <div class="pr-7 pl-2 py-5">
          <h3 class="font-bold">Fast Delivery</h3>
          <p class="text-gray-600 leading-relaxed">30 mins delivery</p>
        </div>
      </div>
      <div class="hidden md:flex justify-end space-x-1 font-bold">
        <span>Powered by</span>
        <FuelerIcon class="w-6 h-6 text-gray-900 fill-current" />
        <span>Fueler</span>
      </div>
    </div>
  </div>
</template>
