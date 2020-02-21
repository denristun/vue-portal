<template>
  <v-app>
    <v-navigation-drawer app></v-navigation-drawer>

    <v-app-bar app></v-app-bar>

    <v-content>
      <v-container fluid>
        <router-view></router-view>
      </v-container>
    </v-content>

    <v-footer app></v-footer>
  </v-app>
</template>

<script>
import Config from "./plugins/config";
export default {
  name: "App",

  components: {},

  data: () => ({
    SITE_NAME: Config.SITE_NAME,
    drawer: false
  })
};
</script>
