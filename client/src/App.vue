<template>
  <v-app>
    <v-app-bar class="blue" app>
      <v-app-bar-nav-icon @click.stop="drawer = !drawer" class="white--text"></v-app-bar-nav-icon>
      <span class="white--text title">Layout Demo</span>
    </v-app-bar>
    <v-navigation-drawer app hide-overlay disable-resize-watcher permanent v-model="drawer">
      <v-list-item>
        <v-list-item-content>
          <v-list-item-title class="text-h6">
            Menu
          </v-list-item-title>
          <v-list-item-subtitle>
            Please select
          </v-list-item-subtitle>
          <v-btn class="" text @click="drawer = false">Close</v-btn>
        </v-list-item-content>
      </v-list-item>
      <v-divider></v-divider> 

      <v-list-item-group>
        <v-list-item active-class="blue" to="/" exact>Home</v-list-item>
        <v-list-item active-class="blue" to="/products" exact>Products</v-list-item>
        <v-list-item active-class="blue" to="/team" exact>Team</v-list-item>
        <v-list-item active-class="blue" to="/about" exact>About</v-list-item>
      </v-list-item-group>
    </v-navigation-drawer>
    <v-main> <router-view></router-view> </v-main>
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
