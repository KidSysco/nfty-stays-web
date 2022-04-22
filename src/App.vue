<template>
  <v-app class="styles-bg-main">
    <v-app-bar app color="black" dark>
      <div class="d-flex align-center pink--text text--accent-2 text-h4">
        <v-img
          src="/img/icons/android-chrome-maskable-192x192.png"
          width="31"
          class="mr-5 ml-2"
        ></v-img>
        <span class="d-none d-sm-none d-md-flex">NFTY STAYS</span>
      </div>

      <v-spacer></v-spacer>

      <!-- <img src="/img/discord.png" class="mx-4" /> -->
      <a
        title="Follow Us on Twitter"
        href="https://twitter.com/NFTyStays"
        target="_new"
        class="mt-2 mx-2"
        ><img src="/img/twitter.png"
      /></a>
      <a
        title="Follow Us on Instagram"
        href="https://www.instagram.com/nftystays/"
        target="_new"
        class="mt-2 mx-2"
        ><img src="/img/instagram.png"
      /></a>
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
