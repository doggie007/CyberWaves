<template>
  <v-content>
    <section id="our-vision">
      <v-container
        fluid
        class="pa-10"
        style="
          background-image: linear-gradient(to bottom left, #dbfcff, #fddcc356);
        "
        :style="{ height: 'calc(100vh - ' + $vuetify.application.top + 'px)' }"
      >
        <v-layout fill-height>
          <v-flex align-self-center class="d-flex justify-center">
            <v-img
              height="600"
              width="20vw"
              min-width="250"
              max-width="400"
              transition="slide-x-transition"
              :src="require('../assets/rocky-beach.jpg')"
            ></v-img>
          </v-flex>
          <v-flex
            align-self-center
            class="d-flex justify-center"
            style="margin-left: -300px"
          >
            <v-card
              outlined
              class="rounded-tl-xl rounded-br-xl"
              width="90%"
              max-width="800"
              color="#274156"
              dark
            >
              <v-card-title
                class="display-2 font-weight-bold mb-3 text-uppercase"
                >Our Vision</v-card-title
              >
              <v-card-subtitle>
                <v-responsive class="mb-0" width="56">
                  <v-divider
                    class="mb-1"
                    style="background: whitesmoke"
                  ></v-divider>
                  <v-divider style="background: white"></v-divider>
                </v-responsive>
              </v-card-subtitle>
              <p class="title font-weight-light pa-2 text-justify">
                We envision a better world where technology helps us to bridge
                the gap between our desire for a healthy planet and achievable +
                actionable solutions. We hope that through education and
                demonstrating the power of current technology, we can empower
                communities to be fearless at solving the ocean pollution
                problem themselves.
              </p>
              <v-btn
                class="ma-3 align-self-center"
                fab
                outlined
                @click="$vuetify.goTo('#five-principles')"
              >
                <v-icon>mdi-chevron-double-down</v-icon>
              </v-btn>
            </v-card>
          </v-flex>
        </v-layout>
      </v-container>
    </section>

    <section id="five-principles">
      <v-container fluid style="height: 100vh">
        <v-layout fill-height>
          <h1>Hi</h1>
        </v-layout>
      </v-container>
    </section>
  </v-content>
</template>
<script>
export default {
  data() {
    return {};
  },
};
</script>
