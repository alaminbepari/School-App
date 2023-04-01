<template>
  <q-page class="q-pa-lg">
    <div class="q-mb-lg">
      <summarySection />
    </div>
    <div class="row q-col-gutter-lg">
      <div class="col-lg-6 col-md-12 col-xs-12 col-12">
        <topstudentSection />
      </div>
      <div class="q-mb-lg col-lg-6 col-md-12 col-xs-12 col-12">
        <studentActivity />
      </div>
    </div>
    <div>
      <socialSection />
    </div>
  </q-page>
</template>

<script setup>
import socialSection from "src/components/dashbord/admin/socialSection.vue";
import topstudentSection from "src/components/dashbord/admin/topstudentSection.vue";
import summarySection from "src/components/dashbord/admin/summarySection.vue";
import studentActivity from "src/components/dashbord/admin/studentActivity.vue";
</script>

<style scoped></style>
