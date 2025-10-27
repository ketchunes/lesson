<template>
  <div class="px-28 py-10">
    <div class="text-black text-3xl font-semibold">Reading blog list</div>
    <div class="grid grid-cols-4 gap-20 mt-10">
      <div class="cursor-pointer transition-transform duration-200 ease-in-out active:scale-95" v-for="list in lists">
        <img class="w-full h-full rounded-xl" :src="list.img" alt="" />
      </div>
    </div>
  </div>
</template>

<script setup>
  const lists = [
    {
      img: "img/ui.png",
    },
    {
      img: "img/react.png",
    },
    {
      img: "img/php.png",
    },
    {
      img: "img/js.png",
    },
  ];
</script>
