<template>
  <v-parallax
    scale="1.4"
    height="100vh"
    class="responsive-portrait"
    src="/assets/img/london.jpg"
    ><div class="logo"><img src="/assets/img/logoem.png" alt="logo" /></div>
  </v-parallax>
  <v-parallax scale="1.5" dark src="/assets/img/backgroundrombos.jpg">
    <v-row>
      <v-col
        v-for="url in photos"
        :key="url"
        class="d-flex child-flex"
        cols="6"
      >
        <v-img
          :src="url"
          :lazy-src="url"
          class="grey lighten-2"
          @click="openImage(url)"
        >
          <template v-slot:placeholder>
            <v-row class="fill-height" align="center" justify="center">
              <v-progress-circular
                indeterminate
                color="grey lighten-5"
              ></v-progress-circular>
            </v-row>
          </template>
        </v-img>
      </v-col>
    </v-row>
    <v-dialog
      v-model="dialog"
      hide-overlay
      overlay-color="black"
      overlay-opacity="50"
    >
      <v-card>
        <img
          :src="currentImg"
          alt="img"
          style="max-width: -webkit-fill-available"
        />
        <v-card-actions>
          <v-btn color="#3466aa" block @click="closeImage(url)">X</v-btn>
        </v-card-actions>
      </v-card>
    </v-dialog>
  </v-parallax>
</template>

<style scoped>
.logo {
  text-align: center;
  margin-top: 7%;
}

.logo img {
  height: 75vh;
}

@media (max-width: 900px) {
  .logo {
    text-align: center;
    display: flex;
    justify-content: center;
    margin-top: 150px;
  }

  .logo img {
    height: 50vh;
  }
}
</style>

<script>
export default {
  data: () => ({
    photos: [
      "/assets/img/photos/photo1.jpg",
      "/assets/img/photos/photo2.jpg",
      "/assets/img/photos/photo3.jpg",
      "/assets/img/photos/photo4.jpg",
      "/assets/img/photos/photo5.jpg",
      "/assets/img/photos/photo6.jpg",
      "/assets/img/photos/photo7.jpg",
      "/assets/img/photos/photo8.jpg",
      "/assets/img/photos/photo9.jpg",
      "/assets/img/photos/photo10.jpg",
    ],

    currentImg: "https://picsum.photos/500/300?image=15",

    dialog: false,
  }),
  methods: {
    openImage(url) {
      this.dialog = true;
      this.currentImg = url;
    },

    closeImage() {
      this.dialog = false;
    },
  },
};
</script>