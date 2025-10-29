<template>
  <div class="py-10">
    <div class="text-center font-semibold text-6xl text-accent-content">Affordable pricing</div>
    <div class="flex justify-center mt-10 gap-5">
      <div class="text-black" v-for="price in prices">
        <div class="card w-96 bg-base-100 shadow-sm">
          <div class="card-body">
            <span class="badge badge-xs badge-warning">{{ price.ind }}</span>
            <div class="flex justify-between">
              <h2 class="text-3xl font-bold">{{ price.price }}</h2>
            </div>
            <ul class="mt-6 flex flex-col gap-2 text-base">
              <li>
                <svg xmlns="http://www.w3.org/2000/svg" class="size-4 me-2 inline-block text-success" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7" />
                </svg>
                <span>{{ price.component1 }}</span>
              </li>
              <li>
                <svg xmlns="http://www.w3.org/2000/svg" class="size-4 me-2 inline-block text-success" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7" />
                </svg>
                <span>{{ price.component2 }}</span>
              </li>
              <li>
                <svg xmlns="http://www.w3.org/2000/svg" class="size-4 me-2 inline-block text-success" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7" />
                </svg>
                <span>{{ price.component3 }}</span>
              </li>
              <li>
                <svg xmlns="http://www.w3.org/2000/svg" class="size-4 me-2 inline-block text-success" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7" />
                </svg>
                <span>{{ price.component4 }}</span>
              </li>
              <li>
                <svg xmlns="http://www.w3.org/2000/svg" class="size-4 me-2 inline-block text-success" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7" />
                </svg>
                <span>{{ price.component5 }}</span>
              </li>
            </ul>
            <div class="mt-6">
              <button class="btn text-base-100 btn-block">Subscribe</button>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
  const prices = [
    {
      ind: "Like a pussy",
      price: "Free / forever",
      component1: "Components-driven system",
      component2: "Sales-boosting landing pages",
      component3: "Awesome Feather icons pack",
      button: "Try for free",
    },
    {
      ind: "individual",
      price: "$24 / moth",
      component1: "Components-driven system",
      component2: "Sales-boosting landing pages",
      component3: "Awesome Feather icons pack",
      component4: "Themed into 3 different styles",
      component5: "Will help to learn Figma",
      button: "Regular license",
    },
    {
      ind: "Corporate",
      price: "$12 / editor",
      component1: "Components-driven system",
      component2: "Sales-boosting landing pages",
      component3: "Awesome Feather icons pack",
      component4: "Themed into 3 different styles",
      button: "Extended license",
    },
  ];
</script>
