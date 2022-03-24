<template>
  <v-container>
    <v-row>
      <v-col cols="12" sm="6" class="d-flex align-center">
        <v-img src="/img/nfty-stays-logo.png" class="mr-8"></v-img>
      </v-col>
      <v-col cols="12" sm="6">
        <v-img src="/img/hero-01.png"></v-img>
      </v-col>
    </v-row>
    <v-row class="mt-12">
      <v-col class="text-h3 text-center"> WHO IS NFTY-STAYS FOR? </v-col>
    </v-row>
    <v-row>
      <v-col cols="12" sm="6" xl="3">
        <v-card class="mx-auto rounded-xl" color="amber darken-2 elevation-7">
          <v-img src="/img/vr-2.jpg" height="200" class=""></v-img>
          <v-card-actions
            ><v-card-title>Investors</v-card-title>
            <v-spacer></v-spacer>
            <v-btn
              text
              large
              @click="isInvestorExpandShowing = !isInvestorExpandShowing"
              >Explore
              <v-icon class="ml-2">{{
                isInvestorExpandShowing ? "mdi-chevron-up" : "mdi-chevron-down"
              }}</v-icon>
            </v-btn>
          </v-card-actions>
          <v-expand-transition>
            <div v-show="isInvestorExpandShowing" class="white">
              <v-divider></v-divider>
              <v-card-text>
                Future Monetization and Tokenization Projects
              </v-card-text>
            </div>
          </v-expand-transition>
        </v-card>
      </v-col>
      <v-col cols="12" sm="6" xl="3">
        <v-card class="mx-auto rounded-xl" color="lime lighten-2">
          <v-img src="/img/vr-4.jpg" height="200" class="align-end"></v-img>
          <v-card-actions
            ><v-card-title>Host</v-card-title>
            <v-spacer></v-spacer>
            <v-btn
              text
              large
              @click="isHostExpandShowing = !isHostExpandShowing"
              >Explore
              <v-icon class="ml-2">{{
                isHostExpandShowing ? "mdi-chevron-up" : "mdi-chevron-down"
              }}</v-icon>
            </v-btn>
          </v-card-actions>
          <v-expand-transition>
            <div v-show="isHostExpandShowing" class="white">
              <v-divider></v-divider>
              <v-card-text>
                Future Franchisee opportunities to increase demand and ROI
              </v-card-text>
            </div>
          </v-expand-transition>
        </v-card>
      </v-col>
      <v-col cols="12" sm="6" xl="3">
        <v-card class="mx-auto rounded-xl" color="light-blue lighten-2">
          <v-img src="/img/vr-3.jpg" height="200"></v-img>
          <v-card-actions
            ><v-card-title>Guests</v-card-title>
            <v-spacer></v-spacer>
            <v-btn
              text
              large
              @click="isGuestExpandShowing = !isGuestExpandShowing"
              >Explore
              <v-icon class="ml-2">{{
                isGuestExpandShowing ? "mdi-chevron-up" : "mdi-chevron-down"
              }}</v-icon>
            </v-btn>
          </v-card-actions>
          <v-expand-transition>
            <div v-show="isGuestExpandShowing" class="white">
              <v-divider></v-divider>
              <v-card-text>
                All Travelers & Guest will love our experiences. Web3/NFT
                Newcomers and Vets alike. Builders, Investors, and Digital
                Nomads. escape.
              </v-card-text>
            </div>
          </v-expand-transition>
        </v-card>
      </v-col>
      <v-col cols="12" sm="6" xl="3">
        <v-card class="mx-auto rounded-xl" color="pink lighten-4">
          <v-img src="/img/vr-1.jpg" height="200"></v-img>
          <v-card-actions
            ><v-card-title>Real Estate</v-card-title>
            <v-spacer></v-spacer>
            <v-btn
              text
              large
              @click="isRealEstateExpandShowing = !isRealEstateExpandShowing"
              >Explore
              <v-icon class="ml-2">{{
                isRealEstateExpandShowing
                  ? "mdi-chevron-up"
                  : "mdi-chevron-down"
              }}</v-icon>
            </v-btn>
          </v-card-actions>
          <v-expand-transition>
            <div v-show="isRealEstateExpandShowing" class="white">
              <v-divider></v-divider>
              <v-card-text
                >Project STOIC- Real Estate Education and Investment NFT Project
              </v-card-text>
            </div>
          </v-expand-transition>
        </v-card>
      </v-col>
    </v-row>
    <v-row class="mt-16">
      <v-col class="text-h3 text-center"> NFTY STAYS MISSION </v-col>
    </v-row>
    <v-row class="d-flex flex-wrap justify-center">
      <v-col cols="12" sm="6" md="4" lg="2" xl="2">
        <v-card color="lime lighten-2" class="black--text" dark>
          <v-card-title class="text-h5"> Immersion </v-card-title>
          <v-card-subtitle class="black--text"
            >Immerse guest in web3 and NFT experiences</v-card-subtitle
          >
        </v-card>
      </v-col>
      <v-col cols="12" sm="6" md="4" lg="2" xl="2">
        <v-card color="pink lighten-4" class="black--text" dark>
          <v-card-title class="text-h5"> Education </v-card-title>
          <v-card-subtitle class="black--text"
            >Onboard new Travelers, Host, and RE Investors to Web3 and
            NFTs</v-card-subtitle
          >
        </v-card>
      </v-col>
      <v-col cols="12" sm="6" md="4" lg="3" xl="3">
        <v-card color="light-blue lighten-2" class="black--text" dark>
          <v-card-title class="text-h5"> Immersion </v-card-title>
          <v-card-subtitle class="black--text"
            >Build a community of Short Term Rental and Real Estate investors
            via Project STOIC</v-card-subtitle
          >
        </v-card>
      </v-col>
      <v-col cols="12" sm="6" md="4" lg="2" xl="2">
        <v-card color="pink lighten-4" class="black--text" dark>
          <v-card-title class="text-h5"> Yield </v-card-title>
          <v-card-subtitle class="black--text"
            >Develop ancillary income streams for independent
            wealth</v-card-subtitle
          >
        </v-card>
      </v-col>
      <v-col cols="12" sm="6" md="4" lg="2" xl="2">
        <v-card color="lime lighten-2" class="black--text" dark>
          <v-card-title class="text-h5"> Adoption </v-card-title>
          <v-card-subtitle class="black--text"
            >Be the early adopters that set industry standards</v-card-subtitle
          >
        </v-card>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {
  name: "home-view",
  data: () => ({
    isHostExpandShowing: false,
    isInvestorExpandShowing: false,
    isGuestExpandShowing: false,
    isRealEstateExpandShowing: false,
  }),
  components: {},
};
</script>
