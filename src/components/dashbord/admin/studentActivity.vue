<template>
  <div>
    <q-card class="q-pa-md border">
      <div class="row justify-between">
        <div class="text-h6 text-bold">Student Activity</div>
        <div>
          <q-icon class="card text-h5" name="more_vert"></q-icon>
        </div>
      </div>
      <div
        class="row justify-between q-pa-lg items-center"
        v-for="(item, index) in activity"
        :key="index"
      >
        <div class="row">
          <div>
            <div>
              <img class="image" :src="item.img" />
            </div>
          </div>
          <div>
            <div class="text-bold one-2">{{ item.title }}</div>
            <div class="one-1">{{ item.subtitle }}</div>
          </div>
        </div>
        <div class="one">{{ item.lebel }}</div>
      </div>
    </q-card>
  </div>
</template>
<script setup>
const activity = [
  {
    title: "1st place in Chess ",
    subtitle: "John Doe won 1st ' place in Chess '",
    img: "https://preschool.dreamguystech.com/template/assets/img/icons/award-icon-01.svg",
    lebel: "1 day ago",
  },
  {
    title: "Participated in Carrom ",
    subtitle: "Justin Lee participated in Carrom",
    img: "https://preschool.dreamguystech.com/template/assets/img/icons/award-icon-02.svg",
    lebel: "1 day ago",
  },
  {
    title: "Internation conference in St.John School ",
    subtitle: "Justin Leeattended internation conference in St.John School",
    img: "https://preschool.dreamguystech.com/template/assets/img/icons/award-icon-03.svg",
    lebel: "1 day ago",
  },
  {
    title: "Won 1st place in Chess ",
    subtitle: "John Doe won 1st place in Chess",
    img: "https://preschool.dreamguystech.com/template/assets/img/icons/award-icon-04.svg",
    lebel: "1 day ago",
  },
];
</script>

<style scoped>
.card {
  background-color: #64646b28;
  border-radius: 5px;
  width: 20px;
  height: 25px;
}
.image {
  width: 45px;
  height: 45px;
  margin-right: 10px;
  background-color: rgba(138, 151, 151, 0.295);
  padding: 10px;
  border-radius: 5px;
}
.one {
  background-color: #fff9ed;
  padding: 5px;
  border-radius: 5px;
  font-size: 12px;
  color: #80808f;
}
.one-1 {
  margin-top: 8px;
  font-size: 12px;
  color: #80808f;
}
.border {
  border-radius: 15px;
}
</style>
