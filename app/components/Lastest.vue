<template>
  <div class="px-28 py-10">
    <div class="flex items-center flex-col gap-3">
      <div class="text-4xl text-secondary-content font-semibold">Lastest News and Resources</div>
      <div class="text-lg">See the developments that have occurred to TOTC in the world</div>
    </div>
    <div class="flex justify-between mt-5">
      <div class="w-1/2 flex flex-col gap-5">
        <div><img :src="'img/coffee.png'" alt="" /></div>
        <button class="btn w-fit px-10 text-base-100 rounded-2xl">NEWS</button>
        <div class="text-3xl w-4/5">Class adds $30 million to its balance sheet for a Zoom-friendly edtech solution</div>
        <div class="w-4/5 text-lg">Class, launched less than a year ago by Blackboard co-founder Michael Chasen, integrates exclusively...</div>
        <button class="btn w-fit px-10 text-base-100 rounded-2xl">Read more</button>
      </div>
      <div class="w-1/2 flex flex-col gap-10">
        <div class="flex gap-5 items-center" v-for="post in posts">
          <img :src="post.img" alt="" />
          <div class="flex flex-col h-fit gap-5">
            <div class="text-2xl font-semibold">{{ post.title }}</div>
            <div class="text-xl">{{ post.text }}</div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
  const posts = [
    {
      img: "img/coffee-1.png",
      title: "Class Technologies Inc. Closes $30 Million Series A Financing to Meet High Demand",
      text: "Class Technologies Inc., the company that created Class,...",
    },
    {
      img: "img/coffee-2.png",
      title: "Zoom’s earliest investors are betting millions on a better Zoom for schools",
      text: "Zoom was never created to be a consumer product. Nonetheless, the...",
    },
    {
      img: "img/coffee-3.png",
      title: "Former Blackboard CEO Raises $16M to Bring LMS Features to Zoom Classrooms",
      text: "This year, investors have reaped big financial returns from betting on Zoom...",
    },
  ];
</script>
