<template>
  <v-container fluid style="padding: 0">
    
    <v-parallax
      scale="1.4"
      height="100vh"
      class="responsive-portrait"
      src="/assets/img/beach.jpg"
    ></v-parallax>
    <v-parallax
    scale="1.5"
    dark
    src="/assets/img/backgroundrombos.jpg"
  >
    <v-row justify="center" class="mt-16">
       <v-col align-self="center" justify="center" cols="12" sm="12">
        <div class="info-box" style="text-align: -webkit-center">
          <h3>Company</h3>
          <p>La Curacao</p>
          <h3>Role</h3>
          <p>Drone Pilot</p>
        </div>
      </v-col>
      <v-col style="text-align: center" cols="12" sm="12" >
        <iframe
          title="vimeo-player"
          src="https://player.vimeo.com/video/675372376?h=e39ab8026e"
          frameborder="0"
          allowfullscreen
          class="player"
        ></iframe>
      </v-col>
     
    </v-row>
    <v-row justify="center" class="mt-16">
      <v-col align-self="center" justify="center" cols="12" class="info-box" >
        <div  style="text-align: -webkit-center">
          <h3>Company</h3>
          <p>Alba Petroleos</p>
          <h3>Role</h3>
          <p>Video editor</p>
        </div>
      </v-col>
      <v-col style="text-align: center" cols="12" sm="12">
        <iframe
          title="vimeo-player"
          src="https://player.vimeo.com/video/675372376?h=e39ab8026e"
          class="player"
          frameborder="0"
          allowfullscreen
        ></iframe>
      </v-col>
    </v-row>
    <v-row justify="center" class="mt-16">
      <v-col align-self="center" justify="center" cols="12">
        <div class="info-box" style="text-align: -webkit-center">
          <h3>Company</h3>
          <p>La Curacao</p>
          <h3>Role</h3>
          <p>Drone Pilot</p>
        </div>
      </v-col>
      <v-col style="text-align: center" cols="12" sm="12">
        <iframe
          title="vimeo-player"
          src="https://player.vimeo.com/video/675372376?h=e39ab8026e"
          frameborder="0"
          allowfullscreen
          class="player"
        ></iframe>
      </v-col>
      
    </v-row>
    <v-row justify="center" class="mt-16">
      <v-col align-self="center" justify="center" cols="12" class="info-box" sm="12">
        <div  style="text-align: -webkit-center">
          <h3>Company</h3>
          <p>Alba Petroleos</p>
          <h3>Role</h3>
          <p>Video editor</p>
        </div>
      </v-col>
      <v-col style="text-align: center" cols="12" sm="12">
        <iframe
          title="vimeo-player"
          src="https://player.vimeo.com/video/675372376?h=e39ab8026e"
          class="player"
          frameborder="0"
          allowfullscreen
        ></iframe>
      </v-col>
    </v-row>
     <v-row justify="center" class="mt-16 mb-5">
        <v-col align-self="center" justify="center" cols="12" sm="12">
        <div class="info-box" style="text-align: -webkit-center">
          <h3>Company</h3>
          <p>La Curacao</p>
          <h3>Role</h3>
          <p>Drone Pilot</p>
        </div>
      </v-col>
      <v-col style="text-align: center" cols="12" sm="12">
        <iframe
          title="vimeo-player"
          src="https://player.vimeo.com/video/675372376?h=e39ab8026e"
          frameborder="0"
          allowfullscreen
          class="player"
        ></iframe>
      </v-col>
     
    </v-row>
    </v-parallax>
  </v-container>
</template>

<style scoped>
.player {
  width: 640px;
  height: 360px;
  text-align: center;
}

h3 {
  color: #3363a4;
  font-size: 50px;
  text-align: center;
}

p {
  color: #fff;
  font-size: 19px;
  text-align: center;
}

.info-box {
  background-color: #363636;
  border-radius: 15px;
  box-shadow: 0.3rem 0.3rem 1rem rgb(24 24 24 / 30%);
}

.background{
  background-size: cover;
}

@media (max-width: 900px) {
  .responsive-portrait {
    height: 10px;
  }

  .player{
    width: 320px;
  height: 130px;
  text-align: center;
  }
}
</style>

<script>
</script>