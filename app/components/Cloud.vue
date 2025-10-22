<template>
  <div class="py-10 px-10 2xl:px-28">
    <div class="flex flex-col items-center gap-5">
      <div class="text-4xl font-semibold text-secondary-content">All-In-One <span class="text-accent-content">Cloud Software.</span></div>
      <div class="text-center 2xl:w-1/3">TOTC is one powerful online software suite that combines all the tools needed to run a successful school or office.</div>
    </div>
    <div class="grid 2xl:grid-cols-3 mt-5 gap-20 2xl:gap-32">
      <div v-for="card in cards">
        <div class="shadow-lg pb-4 rounded-3xl flex flex-col justify-center gap-3">
          <div><img class="m-auto" :src="card.img" alt="" /></div>
          <div class="w-2/3 m-auto h-20 text-3xl font-simebold text-center flex items-center justify-center text-secondary-content">{{ card.title }}</div>
          <div class="text-center m-auto w-2/3">{{ card.text }}</div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
  const cards = [
    {
      img: "img/doc.png",
      title: "Online Billing, Invoicing, & Contracts",
      text: "Simple and secure control of your organization’s financial and legal transactions. Send customized invoices ",
    },
    {
      img: "img/doc-2.png",
      title: "Easy Scheduling & Attendance Tracking",
      text: "Schedule and reserve classrooms at one campus or multiple campuses. Keep detailed records of student attendance",
    },
    {
      img: "img/doc-3.png",
      title: "Customer Tracking",
      text: "Automate and track emails to individuals or groups. Skilline’s built-in system helps organize your organization ",
    },
  ];
</script>
