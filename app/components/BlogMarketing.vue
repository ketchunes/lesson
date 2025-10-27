<template>
  <div class="bg-base-100 px-28 py-10 text-black">
    <div class="text-3xl font-semibold">Marketing Articles</div>
    <div class="grid grid-cols-4 gap-10">
      <div class="bg-base-100 mt-5 p-5 w-fit rounded-2xl shadow-2xl flex flex-col gap-5" v-for="mark in marks">
        <img class="h-full" :src="mark.img" alt="" />
        <div class="text-2xl">{{ mark.title }}</div>
        <div class="text-lg text-base-content">{{ mark.text }}</div>
        <div class="flex justify-between">
          <div class="flex items-center gap-5">
            <img :src="mark.imgMini" alt="" />
            <div class="text-lg">Lina</div>
          </div>
          <div class="flex items-center gap-3 text-lg font-semibold">
            <div class="line-through text-base-content">{{ mark.price }}</div>
            <div class="font-bold text-accent-content">{{ mark.price2 }}</div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
  const marks = [
    {
      img: "img/coffee.png",
      title: "AWS Certified solutions Architect",
      text: "Lorem ipsum dolor sit amet, consectetur adipising elit, sed do eiusmod tempor",
      imgMini: "img/lina.png",
      price: "$100",
      price2: "$80",
    },
    {
      img: "img/coffee-1.png",
      title: "AWS Certified solutions Architect",
      text: "Lorem ipsum dolor sit amet, consectetur adipising elit, sed do eiusmod tempor",
      imgMini: "img/lina.png",
      price: "$100",
      price2: "$80",
    },
    {
      img: "img/coffee-2.png",
      title: "AWS Certified solutions Architect",
      text: "Lorem ipsum dolor sit amet, consectetur adipising elit, sed do eiusmod tempor",
      imgMini: "img/lina.png",
      price: "$100",
      price2: "$80",
    },
    {
      img: "img/coffee-3.png",
      title: "AWS Certified solutions Architect",
      text: "Lorem ipsum dolor sit amet, consectetur adipising elit, sed do eiusmod tempor",
      imgMini: "img/lina.png",
      price: "$100",
      price2: "$80",
    },
  ];
</script>
