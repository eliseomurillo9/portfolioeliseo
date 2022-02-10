<template>
  <link rel="preconnect" href="https://fonts.googleapis.com" />
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
  <link
    href="https://fonts.googleapis.com/css2?family=Fira+Sans:wght@900&family=Poppins:wght@300;500;700&display=swap"
    rel="stylesheet"
  />
  <link rel="preconnect" href="https://fonts.googleapis.com" />
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
  <link
    href="https://fonts.googleapis.com/css2?family=Fira+Sans:wght@900&family=Montserrat:wght@200,600;900&display=swap"
    rel="stylesheet"
  />
  <v-app style="background-color: red">
    <v-layout style="overflow: hidden">
      <v-app-bar absolute color="deep-purple">
        <v-app-bar-nav-icon @click="drawer = !drawer"></v-app-bar-nav-icon>
      </v-app-bar>
      <v-navigation-drawer v-model="drawer" absolute temporary>
        <v-list dense @click="drawer = false"
          ><v-list-item title="Home" href="#"></v-list-item>
          <v-list-item title="About" href="#about"></v-list-item>
          <v-list-item title="Portfolio"></v-list-item>
          <v-list-item title="Video" link="/about" href="#video"></v-list-item>
          <v-list-item title="Graphic Desing" href="#desings"></v-list-item>
          <v-list-item title="Photography" href="#photography"></v-list-item>
          <v-list-item title="Web Development" href="#video"></v-list-item>
        </v-list>
      </v-navigation-drawer>

      <v-main style="background-color: #171717">
        <router-view />
      </v-main>
    </v-layout>
    <v-footer>
      <v-card
        elevation="0"
        rounded="0"
        width="100%"
        class="bg-grey text-center"
      >
        <v-card-text>
          <v-btn
            class="mx-sm-4"
            icon="mdi-github"
            variant="plain"
            color="white"
            @click="goWebSite('https://github.com/eliseomurillo9')"
          ></v-btn>
          <v-btn
            class="mx-4"
            icon="mdi-instagram"
            variant="plain"
            color="white"
            @click="goWebSite('')"
          ></v-btn>
          <v-btn
            class="mx-4"
            icon="mdi-linkedin"
            variant="plain"
            color="white"
            @click="goWebSite('https://www.linkedin.com/in/eliseomurillo9')"
          ></v-btn>
        </v-card-text>

        <v-divider></v-divider>

        <v-card-text class="text-white">
          {{ new Date().getFullYear() }} — <strong>Josue Murillo</strong>
        </v-card-text>
      </v-card>
    </v-footer>
  </v-app>
</template>

<script>
export default {
  data: () => ({
    drawer: false,
  }),

  methods:{
    goWebSite (site){
      window.open(site, "_blank");

    }
  }
};
</script>

<style>
* {
  padding: 0;
  margin: 0;
}

.v-footer {
  padding: 0;
  background-color: #171717;
}
</style>
