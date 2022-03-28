<template>
  <v-container>
    <v-row>
      <v-col>
        <v-img src="/img/NFTY-STAYS-retro.jpeg" class="rounded-xl"></v-img>
      </v-col>
    </v-row>
    <v-row>
      <v-col cols="12" sm="6" class="d-flex align-center">
        <v-img src="/img/nfty-stays-logo.png" class="mr-8"></v-img>
      </v-col>
      <v-col cols="12" sm="6">
        <v-img src="/img/hero-01.png"></v-img>
      </v-col>
    </v-row>

    <v-row class="mt-12">
      <v-col class="text-h3 text-center styles-orange-text">
        WHAT IS NFTY STAYS?
      </v-col>
    </v-row>
    <v-row class="mb-16">
      <v-col cols="12" sm="6" class="text-h5">
        <p>Immersive short term rental experiences incorporating...</p>
        <ul>
          <li>Web 3 & NFT Art, Music, and Project Showcases</li>
          <li>Virtual Reality</li>
          <li>Augmented Reality</li>
          <li>Metaverse</li>
        </ul>
      </v-col>
      <v-col cols="12" sm="6" class="text-h5">
        <p>Who stays at NFTY STAYS?</p>
        <ul>
          <li>All travelers will want to try our experiences</li>
          <li>Technology Enthusiast: Crypto/NFT/Web3 newcomers and vets</li>
          <li>Builders, Investors, Host, and Digital Nomads</li>
        </ul>
      </v-col>
    </v-row>
    <v-row class="mt-16">
      <v-col class="text-h3 text-center styles-yellow-text">
        HOW TO ENJOY NFTY STAYS
      </v-col>
    </v-row>
    <v-row class="mb-16">
      <v-col cols="12" sm="6" xl="3">
        <v-card class="mx-auto rounded-xl" color="styles-blue">
          <v-img src="/img/vr-3.jpg" height="200"></v-img>
          <v-card-actions
            ><v-card-title>Guests & Travelers</v-card-title>
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
              <v-card-text class="text-h6">
                All Travelers, Guest, and NFTy Stays Fans will be able to book
                our first Proof of Concept Stay beginning in May of 2022 in
                Jacksonville , FL. We will be looking to add 2 more Stays within
                a 5 mile radius of the original Stay by July of 2022. Keep an
                eye on our social media for updates and waitlist.
              </v-card-text>
            </div>
          </v-expand-transition>
        </v-card>
      </v-col>
      <v-col cols="12" sm="6" xl="3">
        <v-card class="mx-auto rounded-xl" color="styles-yellow">
          <v-img src="/img/vr-4.jpg" height="200" class="align-end"></v-img>
          <v-card-actions
            ><v-card-title>Host & Real Estate Professionals</v-card-title>
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
              <v-card-text class="text-h6">
                Once our Proof of Concept Stays are successful, we will begin
                our next phase to scale. We will be offering a tiered franchise
                package to approved rentals and host. We will also be launching
                an educational experience on short term rental investing and
                operations, Project S.T.O.I.C. coming soon.
              </v-card-text>
            </div>
          </v-expand-transition>
        </v-card>
      </v-col>
      <v-col cols="12" sm="6" xl="3">
        <v-card class="mx-auto rounded-xl" color="styles-orange elevation-7">
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
              <v-card-text class="text-h6">
                We will be developing and deploying new monetization avenues
                never before seen or tried in the short term rental or NFT
                space. We will also be bringing other future real estate
                opportunities and ventures.
              </v-card-text>
            </div>
          </v-expand-transition>
        </v-card>
      </v-col>
      <v-col cols="12" sm="6" xl="3">
        <v-card class="mx-auto rounded-xl" color="pink lighten-4">
          <v-img src="/img/vr-1.jpg" height="200"></v-img>
          <v-card-actions
            ><v-card-title>NFT Artist, Projects, & Products</v-card-title>
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
              <v-card-text class="text-h6"
                >Inquire how to bring your work or project into our network.
                Come learn about the the real world utility we could provide
                through showcases and exposure in our stays.
              </v-card-text>
            </div>
          </v-expand-transition>
        </v-card>
      </v-col>
    </v-row>
    <v-row class="mt-16">
      <v-col class="text-h3 text-center styles-blue-text">
        NFTY STAYS MISSION
      </v-col>
    </v-row>
    <v-row class="mb-16">
      <div
        class="mx-4 d-flex flex-wrap justify-center align-center indigo darken-3 pa-12 rounded-xl"
      >
        <v-col cols="12" sm="6" md="4" lg="4" xl="2">
          <v-card
            color="styles-purple"
            class="black--text rounded-xl elevation-4"
            dark
          >
            <v-card-title class="text-h5 styles-purple white--text">
              Onboard
            </v-card-title>
            <v-card-subtitle class="styles-yellow black--text pt-4 mt-0 text-h6"
              >Onboard Travelers, Host, and RE Investors to something new in Web
              3</v-card-subtitle
            >
          </v-card>
        </v-col>
        <v-col cols="12" sm="6" md="4" lg="4" xl="2">
          <v-card
            color="styles-purple"
            class="black--text rounded-xl elevation-4"
            dark
          >
            <v-card-title class="text-h5 white--text"> Immerse </v-card-title>
            <v-card-subtitle class="black--text mt-0 pt-4 text-h6 styles-orange"
              >Immerse guests in web3, and NFT experiences inside and outside of
              NFTY Stays</v-card-subtitle
            >
          </v-card>
        </v-col>
        <v-col cols="12" sm="6" md="4" lg="4" xl="2">
          <v-card
            color=" styles-purple"
            class="black--text rounded-xl elevation-4"
            dark
          >
            <v-card-title class="text-h5 white--text"> Develop </v-card-title>
            <v-card-subtitle class="black--text mt-0 pt-4 text-h6 styles-blue"
              >Build a community of Short Term Rental and Real Estate investors
              via Project STOIC</v-card-subtitle
            >
          </v-card>
        </v-col>
        <v-col cols="12" sm="6" md="4" lg="4" xl="2">
          <v-card
            color="styles-purple"
            class="black--text rounded-xl elevation-4"
            dark
          >
            <v-card-title class="text-h5 white--text">
              Collaborate
            </v-card-title>
            <v-card-subtitle
              class="pink lighten-4 black--text mt-0 pt-4 text-h6"
              >Develop ancillary income streams for independent
              wealth</v-card-subtitle
            >
          </v-card>
        </v-col>
        <v-col cols="12" sm="6" md="4" lg="4" xl="2">
          <v-card
            color="styles-purple"
            class="black--text rounded-xl elevation-4"
            dark
          >
            <v-card-title class="text-h5 white--text"> Leverage </v-card-title>
            <v-card-subtitle class="styles-yellow black--text mt-0 pt-4 text-h6"
              >Be the early adopters that set industry
              standards</v-card-subtitle
            >
          </v-card>
        </v-col>
        <v-col cols="12" sm="6" md="4" lg="4" xl="2">
          <v-card
            color="styles-purple"
            class="black--text rounded-xl elevation-4"
            dark
          >
            <v-card-title class="text-h5 white--text"> Monetize </v-card-title>
            <v-card-subtitle class="styles-orange black--text mt-0 pt-4 text-h6"
              >Be the early adopters that set industry
              standards</v-card-subtitle
            >
          </v-card>
        </v-col>
      </div>
    </v-row>
    <v-row class="mt-16">
      <v-col class="text-h3 text-center styles-pink-text">
        FIRST PROOF OF CONCEPT
      </v-col>
    </v-row>
    <v-row class="mb-16">
      <v-col cols="12" sm="6">
        <v-img src="/img/booshie.jpg" class="rounded-xl"></v-img>
      </v-col>
      <v-col cols="12" sm="6"
        ><v-card color="" class="black--text rounded-xl" dark>
          <v-card-title class="text-h4 styles-pink white--text elevation-4">
            Booshie's Crypto Crib
          </v-card-title>
          <v-card-subtitle class="text-h6 black--text styles-yellow pt-1 mt-0">
            <ul class="mt-6">
              <li>3 bedroom, 1 bathroom Stay</li>
              <li>Performing Short Term Rental</li>
              <li>Operated since 2019 as Lily’s Pad JAX</li>
              <li>Will start rebrand and concept deployment on next vacancy</li>
              <li>April 22</li>
              <li>Booshies CRYPTO PAD</li>
              <li>Be the early adopters that set industry standards</li>
            </ul>
            <div class="text-center my-4">
              <v-btn
                color="#272361"
                x-large
                text
                href="https://rumble.com/vfs2v7-welcome-to-lilys-pad-jax.html"
                target="_new"
                >Learn More
              </v-btn>
            </div>
          </v-card-subtitle>
        </v-card></v-col
      >
    </v-row>
    <v-row class="mt-16">
      <v-col class="text-h3 text-center light-blue--text text--lighten-2">
        THE NEXT NFTY STAYS
      </v-col>
    </v-row>
    <v-row class="mb-16">
      <v-col cols="12" sm="6">
        <v-img src="/img/fl-basement.png" class="rounded-xl"></v-img>
      </v-col>
      <v-col cols="12" sm="6">
        <v-img src="/img/1-bed-1-bath.png" class="rounded-xl"></v-img>
      </v-col>
    </v-row>
    <!--
    <v-row class="mt-12">
      <v-col class="text-h3 text-center orange--text text--lighten-1">
        JUST SCRATCHING THE SURFACE
      </v-col>
    </v-row>
    <v-row>
      <v-col
        ><v-card color="pink lighten-4" class="black--text rounded-xl" dark>
          <div class="d-flex flex-no-wrap justify-space-between">
            <div>
              <v-card-title class="text-h5"> Education </v-card-title>
              <v-card-subtitle class="black--text">
                Web3 ecosystem for STR</v-card-subtitle
              >
            </div>

            <v-avatar class="ma-3" size="125" tile>
              <v-img src="/img/nft-1.jpg"></v-img>
            </v-avatar>
          </div> </v-card
      ></v-col>
    </v-row>
    -->
    <v-row class="mt-16">
      <v-col class="text-h3 text-center lime--text text--lighten-2">
        FOUNDER
      </v-col>
    </v-row>
    <v-row class="mb-16">
      <v-col cols="12" sm="6" class="d-flex align-center text-h5">
        <div>
          <strong>Joshua DeDecker AKA reconwhispers</strong>
          <ul>
            <li>RealEstateInvestor</li>
            <li>Real Estate Operations Specialist</li>
            <li>Founder & CEO of Patriot Property Collective</li>
            <li>
              Founder of
              <a href="https://www.dig-a-hash.com" target="_new">Dig-A-Hash</a>
            </li>
          </ul>
        </div>
      </v-col>
      <v-col cols="12" sm="6">
        <v-img src="/img/founder.png" class="rounded-xl"></v-img>
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
