<template>
  <v-parallax
    scale="1.3"
    height="100vh"
    class="responsive-portrait"
    src="/assets/img/guatemala.jpg"
    ><div class="logo"><img src="/assets/img/logoem.png" alt="logo" /></div>
  </v-parallax>
   <v-parallax scale="1.5" dark src="/assets/img/backgroundrombos.jpg">
  <v-row>
    <v-col v-for="url in photos" :key="url" class="d-flex child-flex" cols="6">
      <v-img
        :src="url"
        :lazy-src="url"
        class="grey lighten-2"
        @click="openImage(url)"
      >
        <template v-slot:placeholder>
          <v-row class="fill-height ma-0" align="center" justify="center" >
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
      overlay-opacity = "50"
    >
      <v-card max-height="560px" max-width="605px">
        <img :src="currentImg" alt="img" style="max-width: -webkit-fill-available;"/>
        <v-card-actions>
          <v-btn color="primary" block @click="closeImage(url)">X</v-btn>
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
      "/assets/img/graphic/graph1.jpg",
      "/assets/img/graphic/graph2.jpg",
      "/assets/img/graphic/graph3.jpg",
      "/assets/img/graphic/graph4.jpg",
      "/assets/img/graphic/graph5.jpg",
      "/assets/img/graphic/graph6.jpg",
      "/assets/img/graphic/graph7.jpg",
      "/assets/img/graphic/graph8.jpg",
      "/assets/img/graphic/graph9.jpg",
      "/assets/img/graphic/graph10.jpg"
    ],

    currentImg: "https://picsum.photos/500/300?image=15",

    dialog: false,
  }),
  methods: {
    openImage(url){
      this.dialog = true;
      this.currentImg= url
    },
    
    closeImage(){
      this.dialog = false;
    }
  }

};
</script>