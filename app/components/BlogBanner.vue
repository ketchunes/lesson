<template>
  <div class="bg-base-300 text-black">
    <div class="px-28 py-10 grid grid-cols-2 gap-32 items-center">
      <div class="flex flex-col gap-5">
        <div class="text-xl font-medium">By Themadbrains in <span class="text-accent-content">inspiration</span></div>
        <div class="w-3/4 text-5xl/15 text-secondary-content font-semibold">Why Swift UI Should Be on the Radar of Every Mobile Developer</div>
        <div class="w-2/3 text-lg text-base-content">
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempos Lorem ipsum dolor sitamet, consectetur adipiscing elit, sed do eiusmod tempor
        </div>
        <NuxtLink to="/price" class="btn rounded-xl w-fit text-base-100 py-5 px-10">Start learning now</NuxtLink>
      </div>
      <img class="w-full" :src="'img/coffee.png'" alt="" />
    </div>
  </div>
</template>

<script setup></script>
