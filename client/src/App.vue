<template>
  <v-app>
    <v-app-bar class="grey lighten-5" height="74" app>
      <img class="mx-2" src="images/ff.png" style="height:150px; margin-top:100px" />
      <span class="text-truncate text-h4 blue-grey--text darken-1" style="font-family: Poppins"
        >A Dog With a Mission</span
      >
      <v-spacer></v-spacer>
      <router-link active-class="red--text" to="/" exact>Home</router-link>
      <router-link active-class="red--text" to="/about" exact class="ml-5">About</router-link>
    </v-app-bar>
    <v-main>
      <div class="d-flex">
        <div style="width:250px"></div>
        <div class="mt-10" style="flex:1"><router-view></router-view></div>
      </div>
    </v-main>
  </v-app>
</template>

<script>
export default {
  name: 'App',

  data: () => ({
    //
  }),
};
</script>
