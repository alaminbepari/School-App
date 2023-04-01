<template>
  <q-card class="q-pa-lg">
    <div class="flex justify-between q-mb-lg">
      <div class="text-h6">Upcoming Lesson</div>
      <div class="text-blue">View Al Cours</div>
    </div>

    <div
      class="flex justify-between q-mb-lg"
      v-for="(item, index) in row"
      :key="index"
    >
      <div class="right">
        <div class="text-bold">{{ item.title }}</div>
        <div>{{ item.subtitle }}</div>
        <div>
          <q-icon name="calendar_month" /> <span>{{ item.date }}</span>
          <q-icon name="schedule" /> <span>{{ item.time }}</span>
        </div>
      </div>
      <div class="left">
        <div class="text-right">{{ item.confirm }}</div>
        <div class="q-mt-md">
          <q-btn
            class="btn"
            color="secondary"
            size="md"
            label="Reschedul"
          ></q-btn>
        </div>
      </div>
    </div>
  </q-card>
</template>
<script setup>
import { datetime } from "@intlify/core-base";

const row = [
  {
    title: "Lesson 300",
    subtitle: "3.1 Ipsuum dolors",
    date: "Sep 5, 2022",
    time: "09:00 - 10:00 am",
    confirm: "Confirm",
    btn: "button",
  },
  {
    title: "Lesson 400",
    subtitle: "4.1 Ipsuum dolors",
    date: "Sep 5, 2022",
    time: "09:00 - 10:00 am",
    confirm: "Confirms",
    btn: "button",
  },
];
</script>
<style scoped>
.btn {
  text-transform: none;
}
</style>
