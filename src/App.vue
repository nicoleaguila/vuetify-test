<template>
  <v-app>
    <v-app-bar app color="red accent-1" dark>
      <v-toolbar-title>Edutecno</v-toolbar-title>
      <v-spacer></v-spacer>
      <v-btn to="/home" text>home</v-btn>
      <v-btn to="/" text>login</v-btn>
    </v-app-bar>
    <v-content>
    <router-view></router-view>
    </v-content>
    <v-card height="150">
    <v-footer
      absolute
      class="font-weight-medium" color="indigo lighten-4">
      <v-col class="text-center" cols="12">
        {{ new Date().getFullYear() }} — <strong>Vuetify</strong>
      </v-col>
    </v-footer>
  </v-card>
  </v-app>
</template>

<script>


export default {
  name: 'App'
};
</script>
