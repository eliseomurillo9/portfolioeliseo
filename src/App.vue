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
    <v-app-bar density="compact" absolute style="background-color: orange">
      <v-app-bar-title>Vuetify</v-app-bar-title>
      <v-spacer></v-spacer>
      <v-btn text><router-link to="/">Home</router-link></v-btn>
      <v-divider inset vertical></v-divider>
      <v-btn class="mr-sm-3" text
        ><router-link to="/about">About</router-link></v-btn
      >
      <v-btn class="mr-sm-3" text
        ><router-link to="/portfolio">portfolio</router-link></v-btn
      >
      <v-btn class="mr-sm-3" text
        ><router-link to="/Desings">Desings</router-link></v-btn
      >
      <v-btn class="mr-sm-3" text
        ><router-link to="/photography">photography</router-link></v-btn
      >
      <v-btn class="mr-sm-3" text
        ><router-link to="/video">Video</router-link></v-btn
      >
      <v-btn variant="fill" icon="mdi-dots-vertical" color="white">
        <v-icon>mdi-format-list-bulleted-square</v-icon>
      </v-btn>
    </v-app-bar>
    <v-main style="background-color: #171717">
      <router-view />
    </v-main>
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
          ></v-btn>
          <v-btn
            class="mx-4"
            icon="mdi-instagram"
            
            variant="plain"
            color="white"
          ></v-btn>
          <v-btn
            class="mx-4"
            icon="mdi-linkedin"
            href="www.linkedin.com/in/eliseomurillo9"
            target="_blank"
            variant="plain"
            color="white"
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
