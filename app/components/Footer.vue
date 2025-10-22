<template>
  <div class="bg-secondary-content flex flex-col items-center gap-10 py-10 text-base-100">
    <div class="flex items-center gap-10">
      <img :src="'img/logo.png'" alt="" />
      <div class="text-4xl">|</div>
      <div class="text-2xl">Virtual Class for Zoom</div>
    </div>
    <div class="flex flex-col gap-5">
      <div class="text-3xl">Subscribe to get our Newsletter</div>
      <div class="flex gap-4">
        <input class="input bg-transparent rounded-2xl border-2" type="text" placeholder="Type here" />
        <div class="btn rounded-2xl px-5 text-base-100">Subscribe</div>
      </div>
    </div>
    <div class="flex gap-5 text-lg">
      <div>Careers</div>
      <div>|</div>
      <div>Privacy Policy</div>
      <div>|</div>
      <div>Terms & Conditions</div>
    </div>
    <div>© 2021 Class Technologies Inc.</div>
  </div>
</template>

<script setup></script>
