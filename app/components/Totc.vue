<template>
  <div class="flex justify-center flex-col items-center gap-6 pb-10 px-10 md:px-16">
    <h1 class="text-4xl font-semibold text-secondary-content">What is <span class="text-accent-content">TOTC?</span></h1>
    <p class="lg:w-3/4 2xl:w-1/3 text-center text-base-content">
      TOTC is a platform that allows educators to create online classes whereby they can store the course materials online; manage assignments, quizzes and exams; monitor due dates; grade results and
      provide students with feedback all in one place.
    </p>
    <div class="flex justify-between flex-col gap-10 lg:flex-row 2xl:gap-20">
      <div v-for="elem in tot" class="rounded-2xl relative overflow-hidden">
        <img class="size-full object-cover" :src="elem.img" alt="" />
        <div class="absolute z-10 top-0 left-0 size-full grid place-content-center gap-2">
          <div class="text-3xl text-base-100">{{ elem.title }}</div>
          <div class="btn bg-base-100 border-0 rounded-2xl w-full py-5 m-auto">{{ elem.link }}</div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
  const tot = [
    {
      img: "img/tot.png",
      title: "FOR INSTRUCTORS",
      link: "Start a class today",
    },
    {
      img: "img/tot-1.png",
      title: "FOR STUDENTS",
      link: "Enter access code",
    },
  ];
</script>
