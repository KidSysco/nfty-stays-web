<template>
  <v-app class="styles-bg-main">
    <v-app-bar app color="black" dark>
      <div class="d-flex align-center pink--text text--accent-2 text-h4">
        <v-img
          src="/img/icons/android-chrome-maskable-192x192.png"
          width="31"
          class="mr-5 ml-2"
        ></v-img>
        NFTY STAYS
      </div>

      <v-spacer></v-spacer>

      <img src="/img/discord.png" class="mx-4" />
      <img src="/img/twitter.png" class="mx-4" />
      <img src="/img/instagram.png" class="mx-4" />
    </v-app-bar>

    <v-main>
      <router-view />
    </v-main>
  </v-app>
</template>

<script>
export default {
  name: "App",

  data: () => ({
    //
  }),
};
</script>
