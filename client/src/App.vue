<template>
  <v-app>
    <v-app-bar class="blue" app>
      <v-app-bar-nav-icon class="white--text"></v-app-bar-nav-icon>
      <v-app-bar-title class="white--text">Layout Demo</v-app-bar-title>
    </v-app-bar>
    <v-main class="yellow lighten-4">
      <v-container class="mt-10" style="height: 300px">
        <v-toolbar dense>
          <v-btn icon>
            <v-icon>mdi-content-cut</v-icon>
          </v-btn>
          <v-btn icon>
            <v-icon>mdi-content-paste</v-icon>
          </v-btn>
          <v-btn icon>
            <v-icon>mdi-pencil-outline</v-icon>
          </v-btn>
          <v-btn icon>
            <v-icon>mdi-export-variant</v-icon>
          </v-btn>
          <v-spacer></v-spacer>
          <v-btn icon>
            <v-icon>mdi-dots-vertical</v-icon>
          </v-btn>
        </v-toolbar>
        <v-textarea
          outlined
          class="mt-10"
          label="My Statement"
          value="I wish I had learned Vuetify earlier!"
        ></v-textarea>
      </v-container>
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
