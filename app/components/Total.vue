<template>
  <div class="py-20 px-10 md:px-16 2xl:px-28">
    <div class="flex flex-col items-center gap-5">
      <div class="text-5xl font-bold">Our Success</div>
      <div class="w-4/5 2xl:w-2/5 text-center">
        Ornare id fames interdum porttitor nulla turpis etiam. Diam vitae sollicitudin at nec nam et pharetra gravida. Adipiscing a quis ultrices eu ornare tristique vel nisl orci.
      </div>
    </div>
    <div class="grid grid-cols-2 lg:grid-cols-3 xl:grid-cols-5 justify-center items-center gap-10 mt-20">
      <div class="flex flex-col items-center gap-4" v-for="lol in lols" :key="lol.img">
        <img :src="lol.img" alt="" />
        <div class="text-xl 2xl:text-3xl">{{ lol.text }}</div>
      </div>
    </div>
  </div>
</template>

<script setup>
  const lols = [
    {
      img: "img/15K+.png",
      text: "Students",
    },
    {
      img: "img/75.png",
      text: "Total success",
    },
    {
      img: "img/35.png",
      text: "Main questions",
    },
    {
      img: "img/26.png",
      text: "Chief experts",
    },
    {
      img: "img/16.png",
      text: "Years of experience",
    },
  ];
</script>
