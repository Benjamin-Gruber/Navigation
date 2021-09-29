<template>
  <v-app>
    <v-app-bar class="grey lighten-5" height="74" app>
      <img class="mx-2" src="images/ff.png" style="height:150px; margin-top:100px" />
      <span class="text-truncate text-h4 blue-grey--text darken-1" style="font-family: Poppins"
        >A Dog With a Mission</span
      >
      <v-spacer></v-spacer>
      <v-btn active-class="warning" to="/" exact>Home</v-btn>
      <v-btn active-class="warning" to="/products" exact class="ml-5">Products</v-btn>
      <v-btn active-class="warning" to="/about" exact class="ml-5">About</v-btn>
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
