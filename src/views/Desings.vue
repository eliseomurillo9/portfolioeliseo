<template>
  <v-parallax
    scale="1.3"
    height="100vh"
    width="100vw"
    src="/assets/img/campamento.jpg"
  ></v-parallax>
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
      <v-card>
        <img :src="currentImg" alt="img" style="max-width: -webkit-fill-available;"/>
        <v-card-actions>
          <v-btn color="primary" block @click="closeImage(url)">Close Dialog</v-btn>
        </v-card-actions>
      </v-card>
    </v-dialog>
</template>

<style scoped>
</style>

<script>
export default {
  data: () => ({
    photos: [
      "/assets/img/cuba.jpeg",
      "https://picsum.photos/500/300?image=20",
      "https://picsum.photos/500/300?image=25",
      "https://picsum.photos/500/300?image=30",
      "https://picsum.photos/500/300?image=15",
      "https://picsum.photos/500/300?image=15",
      "https://picsum.photos/500/300?image=15",
      "https://picsum.photos/500/300?image=15",
      "https://picsum.photos/500/300?image=15",
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