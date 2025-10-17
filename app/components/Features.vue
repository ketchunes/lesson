<template>
  <div class="px-28">
    <div class="flex flex-col items-center gap-5">
      <div class="text-4xl font-semibold"><span class="text-secondary-content">Our</span> <span class="text-accent-content">Features</span></div>
      <div class="text-lg">This very extraordinary feature, can make learning activities more efficient</div>
    </div>
    <div class="flex items-center justify-between">
      <img :src="'img/group.png'" alt="" />
      <div class="flex flex-col gap-10">
        <div class="text-4xl text-secondary-content font-semibold w-2/3">A <span class="text-accent-content">user interface</span> designed for the classroom</div>
        <div class="flex gap-5" v-for="icon in icons">
          <div class="w-14 h-14 shadow-xl flex justify-center items-center rounded-full"><img :src="icon.img" alt="" /></div>
          <div class="text-lg w-1/2">{{ icon.text }}</div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
  const icons = [
    {
      img: "img/svg/clone-1.svg",
      text: "Teachers don’t get lost in the grid view and have a dedicated Podium space.",
    },
    {
      img: "img/svg/clone-2.svg",
      text: "TA’s and presenters can be moved to the front of the class.",
    },
    {
      img: "img/svg/clone-3.svg",
      text: "Teachers can easily see all students and class data at one time.",
    },
  ];
</script>
