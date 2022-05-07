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
      <v-col class="text-center styles-orange-text styles-nfty-title">
        <h1>WHAT IS NFTY STAYS?</h1>
      </v-col>
    </v-row>
    <v-row class="mb-16 orange--text text--lighten-4">
      <v-col cols="12" sm="6" class="">
        <h3 class="mb-4">
          Immersive short term rental experiences incorporating...
        </h3>
        <ul>
          <li>Web 3 & NFT Art, Music, and Project Showcases</li>
          <li>Virtual Reality</li>
          <li>Augmented Reality</li>
          <li>Metaverse</li>
        </ul>
      </v-col>
      <v-col cols="12" sm="6" class="">
        <h3 class="mb-4">Who stays at NFTY STAYS?</h3>
        <ul>
          <li>All travelers will want to try our experiences</li>
          <li>Technology Enthusiast: Crypto/NFT/Web3 newcomers and vets</li>
          <li>Builders, Investors, Host, and Digital Nomads</li>
        </ul>
      </v-col>
    </v-row>
    <v-row class="mt-16">
      <v-col class="text-center styles-yellow-text styles-nfty-title">
        <h1>HOW TO ENJOY NFTY STAYS</h1>
      </v-col>
    </v-row>
    <v-row class="mb-16">
      <v-col cols="12" sm="6" xl="3">
        <v-card class="mx-auto rounded-xl" color="styles-yellow">
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
                isGuestExpandShowing ? 'mdi-chevron-up' : 'mdi-chevron-down'
              }}</v-icon>
            </v-btn>
          </v-card-actions>
          <v-expand-transition>
            <div v-show="isGuestExpandShowing" class="white">
              <v-divider></v-divider>
              <v-card-text class="">
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
                isHostExpandShowing ? 'mdi-chevron-up' : 'mdi-chevron-down'
              }}</v-icon>
            </v-btn>
          </v-card-actions>
          <v-expand-transition>
            <div v-show="isHostExpandShowing" class="white">
              <v-divider></v-divider>
              <v-card-text class="">
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
        <v-card class="mx-auto rounded-xl" color="styles-yellow elevation-5">
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
                isInvestorExpandShowing ? 'mdi-chevron-up' : 'mdi-chevron-down'
              }}</v-icon>
            </v-btn>
          </v-card-actions>
          <v-expand-transition>
            <div v-show="isInvestorExpandShowing" class="white">
              <v-divider></v-divider>
              <v-card-text class="">
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
        <v-card class="mx-auto rounded-xl styles-yellow">
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
                  ? 'mdi-chevron-up'
                  : 'mdi-chevron-down'
              }}</v-icon>
            </v-btn>
          </v-card-actions>
          <v-expand-transition>
            <div v-show="isRealEstateExpandShowing" class="white">
              <v-divider></v-divider>
              <v-card-text class=""
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
      <v-col class="text-center styles-blue-text styles-nfty-title">
        <h1>NFTY STAYS MISSION</h1>
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
            <v-card-title class="styles-blue"> Onboard </v-card-title>
            <v-card-subtitle class="light-blue lighten-4 black--text pt-4 mt-0">
              <!-- eslint-disable-next-line -->
              Onboard Travelers, Host, and RE Investors to something new in Web
              3
            </v-card-subtitle>
          </v-card>
        </v-col>
        <v-col cols="12" sm="6" md="4" lg="4" xl="2">
          <v-card
            color="styles-purple"
            class="black--text rounded-xl elevation-4"
            dark
          >
            <v-card-title class="styles-blue"> Immerse </v-card-title>
            <v-card-subtitle class="light-blue lighten-4 black--text pt-4 mt-0">
              Immerse guests in unique experiences inside and out of NFTy Stays
            </v-card-subtitle>
          </v-card>
        </v-col>
        <v-col cols="12" sm="6" md="4" lg="4" xl="2">
          <v-card
            color=" styles-purple"
            class="black--text rounded-xl elevation-4"
            dark
          >
            <v-card-title class="styles-blue"> Develop </v-card-title>
            <v-card-subtitle class="light-blue lighten-4 black--text pt-4 mt-0">
              Develop ancillary income streams to create independent wealth
            </v-card-subtitle>
          </v-card>
        </v-col>
        <v-col cols="12" sm="6" md="4" lg="4" xl="2">
          <v-card
            color="styles-purple"
            class="black--text rounded-xl elevation-4"
            dark
          >
            <v-card-title class="styles-blue"> Collaborate </v-card-title>
            <v-card-subtitle class="light-blue lighten-4 black--text pt-4 mt-0">
              <!-- eslint-disable-next-line -->
              Collaborate with Web3, NFT, AR, VR, and Metaverse creators for
              mutual benefit
            </v-card-subtitle>
          </v-card>
        </v-col>
        <v-col cols="12" sm="6" md="4" lg="4" xl="2">
          <v-card
            color="styles-purple"
            class="black--text rounded-xl elevation-4"
            dark
          >
            <v-card-title class="styles-blue"> Leverage </v-card-title>
            <v-card-subtitle class="light-blue lighten-4 black--text pt-4 mt-0">
              Leverage new technologies to enhance every aspect of our Stays
            </v-card-subtitle>
          </v-card>
        </v-col>
        <v-col cols="12" sm="6" md="4" lg="4" xl="2">
          <v-card
            color="styles-purple"
            class="black--text rounded-xl elevation-4"
            dark
          >
            <v-card-title class="styles-blue"> Monetize </v-card-title>
            <v-card-subtitle class="light-blue lighten-4 black--text pt-4 mt-0">
              Monetization opportunities in creative and innovative ways
            </v-card-subtitle>
          </v-card>
        </v-col>
      </div>
    </v-row>
    <v-row class="mt-16">
      <v-col class="text-center styles-pink-text styles-nfty-title">
        <h1>Featured Projects</h1>
      </v-col>
    </v-row>
    <v-row>
      <v-col>
        <v-card
          color="styles-purple"
          class="black--text rounded-xl elevation-4 mb-4"
          dark
        >
          <v-img src="/img/inside-01.jpg" max-height="300"></v-img>
          <v-card-title class="styles-pink white--text">
            The "Stay NFTy" Landscape Art NFT
          </v-card-title>
          <v-card-text class="purple lighten-4 black--text pt-4 mt-0">
            <p><strong>On sale at OpenSea Now!</strong></p>
            <p>
              Series of 15, 1/1, original, landscape artworks that incorporate
              physical and digital world ownership, proof of concept short term
              rentals, and innovative monetization avenues for NFT artist and
              Projects. Each NFT holder has a unique piece of landscape art,
              ownership of their NFT IP, 6% revenue on any leased IP income, and
              represent 1/15 ownership of the physical art display that will be
              available in one of the 1st proof of concept NFTy Stays.
            </p>
            <p class="mb-0">
              <v-btn
                x-large
                target="_new"
                color="primary"
                href="https://opensea.io/collection/stay-nfty-landscape-art"
              >
                Buy Now on OpenSea
              </v-btn>
            </p>
          </v-card-text>
          <v-card-text
            class="purple lighten-4 black--text pt-4 mt-0 text-center"
          >
            <p>
              Featured Artist: TJSART - Physical Signs by
              <a
                href="https://degendisplays.com?sca_ref=1687629.1Iu3AkQTX1"
                target="_new"
                >Degen Displays</a
              >
              - Presented by
              <a href="https://www.dig-a-hash.com" target="_new"
                >Dig-A Hash Holdings</a
              >
            </p>

            <v-btn
              color="secondary"
              outlined
              class="mb-2"
              small
              @click="isNftExpandShowing = !isNftExpandShowing"
              >Explore TJSART
              <v-icon class="ml-2">{{
                isNftExpandShowing ? 'mdi-chevron-up' : 'mdi-chevron-down'
              }}</v-icon>
            </v-btn>
          </v-card-text>
          <v-expand-transition>
            <div
              v-show="isNftExpandShowing"
              class="grey darken-3 pink--text text--lighten-4"
            >
              <v-row class="mx-2">
                <v-col
                  ><h3>TJSART</h3>

                  <v-btn href="https://opensea.io/TJSART" target="_new"
                    >https://opensea.io/TJSART</v-btn
                  >
                </v-col>
              </v-row>
              <v-row class="mx-2">
                <v-col cols="12" md="6">
                  <v-img src="/img/tjsart.jpg" class="rounded-xl"></v-img
                ></v-col>
                <v-col cols="12" md="6"
                  ><p>
                    My Name is TJ and I am an artist now living in Los Angeles.
                    I am originally from the beautiful country of Guatemala . It
                    is truly a beautiful country but there is also a lot of
                    poverty and hunger.
                  </p>

                  <p>
                    My love for art started when I was kid! I didn't have the
                    easiest childhood growing up as I was raised by an abusive
                    alcoholic step father who kicked me out of the house when I
                    was just 9 years old. I begged for food and water for days
                    until a sweet lady found me lost and wandering in the
                    streets and took me in. She made sure I was fed and taken
                    care of by her friend’s orphanage where I lived for the next
                    5 years.
                  </p>

                  <p>
                    In the summer of 2009, I was adopted by my dad from Los
                    Angeles and moved to Santa Monica, California where I was
                    able to pursue my passion in arts and in started drawing and
                    painting more. I actually won a few awards in high school
                    for my art! After I graduated from high school, I attended
                    art college for two years to pursue digital media motion
                    graphics, graphic design, and fine arts.
                  </p>

                  <p>
                    Today, I’m pursuing NFTs full time because I want to be a
                    part of history and change the world by helping artists and
                    charities such as the fight against hunger and poverty in
                    the world in anyway I can. I came from nothing and I’m
                    blessed to have this new life.
                  </p>
                  <p>
                    It’s time to give back to the world! Thank you for taking
                    the time to read about my life and getting to know me a
                    little bit.
                  </p></v-col
                >
              </v-row>
            </div>
          </v-expand-transition>
        </v-card>
      </v-col>
    </v-row>
    <v-row>
      <v-col class="pink--text text--lighten-4">
        <h2 class="mb-4">NFTy Stays Metaverse House Party</h2>
        <p>
          Welcome to the vision of the NFTy Stay Metaverse House Party featuring
          our custom theme song "Stay NFTy" by ProjectLB52 and performed by Dan
          the lost boy.
        </p>
      </v-col>
      <v-col cols="12" sm="6" class="text-center">
        <iframe
          class="styles-rumble rounded-xl"
          src="https://rumble.com/embed/v106tpj/?pub=4"
          frameborder="0"
          allowfullscreen
        ></iframe>
      </v-col> </v-row
    ><v-row
      ><v-col class="pink--text text--lighten-4">
        <h2 class="mb-4">Time Lapse of "Stay NFTy" by TJSART</h2>
        <p>
          This is a time lapse video of "Stay NFTy" by TJSART created for NFTy
          Stays and presented via NFT by Dig-A Hash played to the instrumental
          of Count on Nobody by Arye.
        </p>
        <p></p>
      </v-col>
      <v-col cols="12" sm="6" class="text-center">
        <iframe
          class="styles-rumble rounded-xl"
          src="https://rumble.com/embed/v107oyt/?pub=4"
          frameborder="0"
          allowfullscreen
        ></iframe>
      </v-col>
    </v-row>
    <v-row>
      <v-col>
        <v-card
          color="styles-purple"
          class="black--text rounded-xl elevation-4"
          dark
        >
          <v-img src="/img/nfty-stays-graffiti.jpg"></v-img>

          <v-card-title class="styles-pink white--text">
            NFTy Stays Graffiti NFT
          </v-card-title>
          <v-card-text class="purple lighten-4 black--text pt-4 mt-0">
            Custom graffiti NFT banner by dizzy store! <br />
            <v-btn
              color="primary"
              class="mt-2"
              large
              href="https://objkt.com/asset/KT1BB4iwhidJFHBVVeJcvLMr9wN7viuEiyvw/18"
              target="_new"
              >Explore</v-btn
            >
          </v-card-text>
        </v-card>
      </v-col>
    </v-row>
     <v-row class="mt-16">
      <v-col class="text-center styles-yellow-text styles-nfty-title">
        <h1>Road Map</h1>
      </v-col>
    </v-row>
    <v-row>
      <v-col>
        <v-timeline dark class="styles-yellow-text" align-top :dense="$vuetify.breakpoint.smAndDown">
          <v-timeline-item color="styles-blue" >
            <h3 class="mb-4">Jan-Mar 22</h3>
            <div>
              <ul>
                <li>✅ Research and Branding</li>
                <li>✅ Socials Deployment</li>
                <li>✅ Website 1.0</li>
              </ul>
            </div>
          </v-timeline-item>
          <v-timeline-item color="styles-green">
            <div class="d-flex justify-md-end">
              <div>
                <h3 class="mb-4 text-left text-sm-right">Apr - Jun 22</h3>
                <ul>
                  <li>🚧 App 1.0</li>
                  <li>🚧 Website 2.0</li>
                  <li>🚧 1st Proof of Concept hard/soft launch</li>
                  <li>🔜 2nd Proof of Concept soft launch</li>
                </ul>
              </div>
            </div>
          </v-timeline-item>
          <v-timeline-item color="styles-orange">
            <h3 class="mb-4">Jul - Sep 22</h3>
            <div>
              <ul>
                <li>🔜 2nd Proof of Concept hard launch</li>
                <li>🔜 3rd Proof of Concept soft/hard launch</li>
              </ul>
            </div>
          </v-timeline-item>
          <v-timeline-item color="styles-pink">
            <div class="d-flex justify-md-end">
              <div>
                <h3 class="mb-4 text-left text-sm-right">Oct - Dec 22</h3>
                <ul>
                  <li>🔜 App 2.0</li>
                  <li>🔜 Website 3.0</li>
                  <li>🚧 Project S.T.O.I.C</li>
                </ul>
              </div>
            </div>
          </v-timeline-item>
        </v-timeline>
      </v-col>
    </v-row>
    <v-row class="mt-16">
      <v-col class="text-center styles-orange-text styles-nfty-title">
        <h1>Pitch Deck</h1>
      </v-col>
    </v-row>
    <v-row>
      <v-col>
        <p class="orange--text text--lighten-4">
          Get a look inside, and view the NFTy Stays Pitch Deck by downloading
          the PDF file.
        </p>
        <v-btn color="styles-orange" href="/img/NFTY.STAYS.DECK.pdf" x-large>
          <v-icon class="mr-2">mdi-download</v-icon> Download PDF
        </v-btn>
      </v-col>
    </v-row>
    <v-row class="my-16">
      <v-col>
        <hr class="white" />
      </v-col>
    </v-row>
    <v-row class="mt-16">
      <v-col class="d-flex justify-center flex-wrap">
        <v-img
          src="/img/nfty-stays-logo.png"
          contain
          max-height="80"
          class="my-2"
        ></v-img>
      </v-col>
    </v-row>
    <div class="text-center grey--text text--darken-1 mb-16">
      NFTy Stays <br />
      Copyright 2022
    </div>
  </v-container>
</template>

<script>
export default {
  name: 'home-view',
  data: () => ({
    isHostExpandShowing: false,
    isInvestorExpandShowing: false,
    isGuestExpandShowing: false,
    isRealEstateExpandShowing: false,
    isNftExpandShowing: false,
  }),
  components: {},
};
</script>
