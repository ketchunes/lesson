<template>
  <div class="px-10 py-10 2xl:px-28">
    <div class="grid justify-between items-center grid-rows-2 2xl:grid-cols-2">
      <div class="flex flex-col gap-12 items-center 2xl:items-start">
        <div class="flex items-center gap-3">
          <div class="w-10 h-0.5 bg-base-content"></div>
          <div class="text-xl">TESTIMONIAL</div>
          <div class="w-10 h-0.5 bg-base-content"></div>
        </div>
        <div class="text-3xl text-secondary-content font-semibold 2xl:text-4xl">What They Say?</div>
        <div class="flex flex-col text-lg gap-4 2xl:w-1/2">
          <div>TOTC has got more than 100k positive ratings from our users around the world.</div>
          <div>Some of the students and teachers were greatly helped by the Skilline.</div>
          <div>Are you too? Please give your assessment</div>
          <div class="btn w-fit text-base-100 rounded-2xl m-auto 2xl:m-0">Write your assessment</div>
        </div>
      </div>
      <div><img :src="'img/Gloria.png'" alt="" /></div>
    </div>
  </div>
</template>

<script setup></script>
