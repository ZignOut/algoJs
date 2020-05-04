<template>
  <v-app>
    <div>
      <v-app-bar fixed dense dark color="white">
        <v-btn :ripple="false" text href="/" class="teal--text">
          <h1 class="title">Algo</h1>
          <span class="subtitle1">JS</span>
        </v-btn>
      </v-app-bar>

      <v-content class="pb-10">
        <router-view></router-view>
      </v-content>

      <v-footer dark padless>
          <v-card class="px-12 flex teal darken-3" flat tile>
            <v-card-title>
              <h3 class="title white--text">Join Our Community</h3>

              <v-spacer></v-spacer>

              <v-btn class="mx-4 white--text" icon v-for="icon in icons" :key="icon" :href="icon.link">
                <v-icon size="24px">{{ icon.icon }}</v-icon>
              </v-btn>
            </v-card-title>

            <v-card-text class="text-center pb-0">
              <p class="white--text">
                Developed By
                <a
                  class="yellow--text"
                  href="https://www.kaunghtut.com"
                  style="color: teal; text-decoration: none;"
                >Kaung Htut</a>.
              </p>
            </v-card-text>
          </v-card>
      </v-footer>
    </div>
  </v-app>
</template>

<script>
export default {
  name: "App",

  data: () => ({
    icons: [
      {
        icon: "mdi-facebook",
        link: "www.facebook.com"
      },
      {
        icon: "mdi-github",
        link: "www.github.com"
      },
      {
        icon: "mdi-linkedin",
        link: "www.linkedin.com"
      },
      {
        icon: "mdi-discord",
        link: "www.discord.com"
      }
    ]
  })
};
</script>
