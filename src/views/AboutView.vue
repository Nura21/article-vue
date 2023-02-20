<template>
  <div class="about">
    <div class="container">
      <h3 class="p-3 text-center">Vue.js - List Table</h3>
      <div>
        <v-table class="bg-blue-lighten-1">
          <thead>
            <tr>
              <th class="text-left font-weight-bold">id</th>
              <th class="text-left font-weight-bold">Title</th>
              <th class="text-left font-weight-bold">Description</th>
              <th class="text-left font-weight-bold">Data</th>
              <th class="text-left font-weight-bold">Author</th>
            </tr>
          </thead>
          <tbody>
            <tr v-for="item in desserts" :key="item.name">
              <td>{{ item.id }}</td>
              <td>{{ item.title }}</td>
              <td>{{ item.discription }}</td>
              <td>{{ item.data }}</td>
              <td>{{ item.author }}</td>
            </tr>
          </tbody>
        </v-table>
      </div>
      <div>
        <v-btn variant="tonal" class="mx-8 mt-4">upload</v-btn>
        <v-btn variant="tonal" class="mx-8 mt-4">Edit</v-btn>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      desserts: [
        {
          id: 1,
          title: "Sepeda",
          discription: "transfortasi",
          data: "data masuk",
          author: "faisal",
        },
        {
          id: 2,
          title: "Motor",
          discription: "transfortasi",
          data: "data keluar",
          author: "ayo siapa",
        },
        {
          id: 3,
          title: "Mobil",
          discription: "transfortasi",
          data: "data masuk",
          author: "siapa aja",
        },
      ],
    };
  },
};
</script>

<!-- <style>
@media (min-width: 1024px) {
  .about {
    min-height: 100vh;
    display: flex;
    align-items: center;
  }
}
</style> -->
