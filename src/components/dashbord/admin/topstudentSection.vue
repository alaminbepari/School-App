<template>
  <div>
    <q-card class="q-pa-lg border">
      <div class="row justify-between items-center q-mb-md">
        <div class="text-h6 text-bold">Star Student</div>
        <div class="text-h5 text-bold">
          <q-icon class="bg" name="more_vert"></q-icon>
        </div>
      </div>
      <q-markup-table class="q-pa-sm">
        <thead>
          <tr class="bg-1">
            <td>ID</td>
            <td>Name</td>
            <td>Mark</td>
            <td>Parcentage</td>
            <td>Year</td>
          </tr>
        </thead>
        <tbody>
          <tr class="bg-red q-pa-lg" v-for="(item, index) in row" :key="index">
            <td>{{ item.Id }}</td>
            <td>
              <q-avatar>
                <img
                  style="width: 30px; height: 30px"
                  class="img q-mr-sm"
                  :src="item.image"
                />
              </q-avatar>
              <span>{{ item.name }}</span>
            </td>
            <td>{{ item.mark }}</td>
            <td>{{ item.parcentage }}</td>
            <td>{{ item.year }}</td>
          </tr>
        </tbody>
      </q-markup-table>
    </q-card>
  </div>
</template>

<script setup>
const row = [
  {
    Id: "ABCS11",
    name: "Shuvo Niloy",
    image:
      "https://media.licdn.com/dms/image/D4E03AQEFCncs3ctuVg/profile-displayphoto-shrink_800_800/0/1679665762471?e=2147483647&v=beta&t=kJQCYJolAlA1ePta2ItLKxxx4UKYaX6coMA_0U_h3WA",
    mark: 33,
    parcentage: "70%",
    year: 2019,
  },
  {
    Id: "ABCS11",
    name: "John Smith",
    image:
      "https://preschool.dreamguystech.com/template/assets/img/profiles/avatar-02.jpg",
    mark: 33,
    parcentage: "70%",
    year: 2019,
  },
  {
    Id: "ABCS11",
    name: " Jolie Hoskins",
    image:
      "https://preschool.dreamguystech.com/template/assets/img/profiles/avatar-03.jpg",
    mark: 33,
    parcentage: "70%",
    year: 2019,
  },
  {
    Id: "ABCS11",
    name: "Pennington Joy",
    image:
      "https://preschool.dreamguystech.com/template/assets/img/profiles/avatar-04.jpg",
    mark: 33,
    parcentage: "70%",
    year: 2019,
  },
  {
    Id: "ABCS11",
    name: " Millie Marsden",
    image:
      "https://preschool.dreamguystech.com/template/assets/img/profiles/avatar-05.jpg",
    mark: 33,
    parcentage: "70%",
    year: 2019,
  },
];
</script>

<style scoped>
.bg {
  background-color: #84849125;
  border-radius: 5px;
  width: 20px;
  height: 25px;
}
.bg-1 {
  background-color: #68687025;
}
/* .img {
  display: flex;
  align-items: center;
  justify-content: center;
  border-radius: 20px;
  width: 30px;
  height: 30px;
} */
.border {
  border-radius: 13px;
}
</style>
