<template>
  <div class="px-28 py-10">
    <div class="text-black text-3xl font-semibold">Reading blog list</div>
    <div class="grid grid-cols-4 mt-10">
      <div v-for="list in lists">
        <img :src="list.img" alt="" />
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
