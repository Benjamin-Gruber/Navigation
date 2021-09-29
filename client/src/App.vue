<template>
  <v-app>
    <!-- Aufgabe 1: Nein, da jede Komponente eine feste Position hat. -->

    <!-- Aufgabe 2
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
    </v-main> -->

    <!-- Aufgabe 3
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
    <v-main> <router-view></router-view> </v-main> -->

    <!-- Aufgabe 4, (hier hatte ich etwas hilfe)
    <v-app-bar class="grey lighten-5" height="74" app>
      <img class="mx-2" src="images/ff.png" style="height:150px; margin-top:100px" />
      <span class="text-truncate text-h4 blue-grey--text darken-1" style="font-family: Poppins"
        >A Dog With a Mission</span
      >
      <v-spacer></v-spacer>
      <v-btn active-class="warning" to="/" exact>Home</v-btn>
      <v-btn active-class="warning" to="/products" exact class="ml-5">Products</v-btn>
      <v-btn active-class="warning" to="/about" exact class="ml-5">About</v-btn>

      <v-app-bar-nav-icon
        @click.stop="drawer = !drawer"
        class="white--text d-lg-none blue-grey darken-3"
        v-if="!drawer"
      ></v-app-bar-nav-icon>
    </v-app-bar>
    <v-navigation-drawer app hide-overlay disable-resize-watcher v-model="drawer" right>
      <v-list-item-group>
        <v-list-item>
          <v-list-item-content>
            <v-list-item-title class="text-h6">
              Menu
            </v-list-item-title>
            <v-list-item-subtitle>
              Please select
            </v-list-item-subtitle>
          </v-list-item-content>
          <v-btn text @click="drawer = false" class="blue-grey darken-3 white--text"
            ><v-icon small>
              mdi-close
            </v-icon></v-btn
          >
        </v-list-item>

        <v-divider></v-divider>
        <v-list-item
          link
          v-for="(route, i) in routes"
          :key="i"
          :to="route.link"
          active-class="yellow white--text darken-3"
        >
          {{ route.name }}
        </v-list-item>
      </v-list-item-group>
    </v-navigation-drawer>
    <v-main>
      <div class="d-flex">
        <div style="width:250px"></div>
        <div class="mt-10" style="flex:1"><router-view></router-view></div>
      </div>
    </v-main>
    <v-bottom-navigation
      ><v-btn value="favorites" to="/">
        <v-icon>mdi-home</v-icon>
      </v-btn></v-bottom-navigation
    > -->
  </v-app>
</template>

<script>
export default {
  name: 'App',

  data: () => ({
    drawer: false,
    mini: true,
    routes: [
      { name: 'Home', link: '/' },
      { name: 'Products', link: '/products' },
      { name: 'Team', link: '/team' },
      { name: 'About', link: '/about' },
    ],
  }),
};
</script>
