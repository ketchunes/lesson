<template>
  <div class="bg-base-300 px-28 py-10 text-black">
    <div class="text-3xl font-semibold">Related Blog</div>
    <div class="grid grid-cols-2 gap-20">
      <div class="bg-base-100 flex flex-col gap-5 px-10 mt-10 rounded-2xl py-7" v-for="rel in rels">
        <img :src="rel.img" alt="" />
        <div class="text-xl font-medium">{{ rel.title }}</div>
        <div class="flex items-center gap-5">
          <div><img :src="rel.imgMini" alt="" /></div>
          <div class="text-xl">Lina</div>
        </div>
        <div class="text-lg text-base-content">{{ rel.text }}</div>
        <div class="text-lg text-base-content underline cursor-pointer">Read more</div>
      </div>
    </div>
  </div>
</template>

<script setup>
  const rels = [
    {
      img: "img/tot-2.png",
      imgMini: "img/lina.png",
      title: "Class adds $30 million to its balance sheet for a Zoom-friendly edtech solution",
      text: "Class, launched less than a year ago by Blackboard co-founder Michael Chasen, integrates exclusively...",
    },
    {
      img: "img/coffee.png",
      imgMini: "img/lina.png",
      title: "Class adds $30 million to its balance sheet for a Zoom-friendly edtech solution",
      text: "Class, launched less than a year ago by Blackboard co-founder Michael Chasen, integrates exclusively...",
    },
  ];
</script>
