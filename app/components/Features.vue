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
    <div>
      <div class="grid grid-cols-2 items-center" v-for="(wrap, index) in wraps">
        <div>
          <div class="flex flex-col gap-5">
            <div class="text-secondary-content text-4xl w-2/3 font-semibold">{{ wrap.title }}</div>
            <div class="text-lg w-1/2">{{ wrap.text }}</div>
          </div>
        </div>
        <div :class="{ 'col-start-1 row-start-1': index % 2 === 1 }"><img :src="wrap.img" alt="" /></div>
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
  const wraps = [
    {
      img: "img/woman-1.png",
      title: "Tools For Teachers And Learners",
      text: "Class has a dynamic set of teaching tools built to be deployed and used during class. Teachers can handout assignments in real-time for students to complete and submit.",
    },
    {
      img: "img/wrap.png",
      title: "Assessments, Quizzes, Tests",
      text: "Easily launch live assignments, quizzes, and tests. Student results are automatically entered in the online gradebook.",
    },
    {
      img: "img/wrap-1.png",
      title: "Class Management Tools for Educators",
      text: "Class provides tools to help run and manage the class such as Class Roster, Attendance, and more. With the Gradebook, teachers can review and grade tests and quizzes in real-time.",
    },
    {
      img: "img/wrap-2.png",
      title: "One-on-One Discussions",
      text: "Teachers and teacher assistants can talk with students privately without leaving the Zoom environment.",
    },
  ];
</script>
