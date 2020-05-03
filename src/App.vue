<template>
  <v-app>
    <div>
      <v-app-bar dense dark color="white">
        <v-btn :ripple="false" text href="/" class="teal--text">
          <h1 class="title">Algo</h1>
          <span class="subtitle1">JS</span>
        </v-btn>
      </v-app-bar>

      <v-content>
        <router-view></router-view>
      </v-content>
    </div>
  </v-app>
</template>

<script>
export default {
  name: "App",

  data: () => ({
    //
  })
};
</script>
