<template>
  <v-container fluid style="padding: 0">
    <v-parallax
      scale="1.3"
      height="100vh"
      class="responsive-portrait"
      src="/assets/img/beach.jpg"
      ><div class="logo"><img src="/assets/img/logoem.png" alt="logo" /></div>
    </v-parallax>

    <v-parallax scale="1.5" dark src="/assets/img/backgroundrombos.jpg">
      <v-row justify="center" >
        <v-col align-self="center" justify="center" cols="12" sm="12">
          <div class="info-box" style="text-align: -webkit-center">
            <h3>Company</h3>
            <p>La Curacao</p>
            <h3>Role</h3>
            <p>Drone Pilot</p>
          </div>
        </v-col>
        <v-col style="text-align: center" cols="12" sm="12" class="player-responsive">
          <iframe
            src="https://player.vimeo.com/video/675372376?h=e39ab8026e"
            frameborder="0"
            allowfullscreen
            class="player"
          ></iframe>
        </v-col>
      </v-row>
      <v-row justify="center" class="mt-16">
        <v-col align-self="center" justify="center" cols="12">
          <div class="info-box" style="text-align: -webkit-center">
            <h3>Company</h3>
            <p>Alba Petroleos</p>
            <h3>Role</h3>
            <p>Video editor</p>
          </div>
        </v-col>
        <v-col style="text-align: center" cols="12" sm="12" class="player-responsive mt-n12">
          <iframe
            src="https://player.vimeo.com/video/675373533?h=07ef4f1e30"
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
            <p>COMPAZ</p>
            <h3>Role</h3>
            <p>Editor</p>
          </div>
        </v-col>
        <v-col style="text-align: center" cols="12" sm="12" class="player-responsive mt-n12">
          <iframe
            title="vimeo-player"
            src="https://player.vimeo.com/video/675234558?h=dcc1264ac6"
            frameborder="0"
            allowfullscreen
            class="player"
          ></iframe>
        </v-col>
      </v-row>
      <v-row justify="center" class="mt-16">
        <v-col align-self="center" justify="center" cols="12" sm="12">
          <div class="info-box" style="text-align: -webkit-center">
            <h3>Company</h3>
            <p>B&C Luxury Auto</p>
            <h3>Role</h3>
            <p>Video editor</p>
          </div>
        </v-col>
        <v-col style="text-align: center" cols="12" sm="12" class="player-responsive mt-n12">
          <iframe
            src="https://player.vimeo.com/video/675234486?h=8cc149a2cc"
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
            <p>COMPAZ</p>
            <h3>Role</h3>
            <p>Director, Video editor and Drone Pilot</p>
          </div>
        </v-col>
        <v-col style="text-align: center" cols="12" sm="12" class="player-responsive mt-n12">
          <iframe
            src="https://player.vimeo.com/video/675372086?h=6408444000"
            frameborder="0"
            allowfullscreen
            class="player"
          ></iframe>
        </v-col>
      </v-row>
      <v-row justify="center" class="mt-16 mb-5">
        <v-col align-self="center" justify="center" cols="12" sm="12">
          <div class="info-box" style="text-align: -webkit-center">
            <h3>Showreel</h3>
          </div>
        </v-col>
        <v-col style="text-align: center" cols="12" sm="12" class="player-responsive mt-n12">
          <iframe
            src="https://player.vimeo.com/video/676198222?h=b50d88d461"
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
  width: 1080px;
  height: 720px;
  text-align: center;
}

h3 {
  color: #3363a4;
  font-size: 50px;
  text-align: center;
  font-family: Montserrat;
  font-weight: 700;
}

p {
  color: #fff;
  font-size: 19px;
  text-align: center;
  font-family: Montserrat;
  font-weight: 300;
}

.info-box {
  background-color: #363636;
  box-shadow: 0.3rem 0.3rem 1rem rgb(24 24 24 / 30%);
}

.background {
  background-size: cover;
}
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
  .responsive-portrait {
    height: 10px;
  }

  .player-responsive{
    display: flex;
    justify-content: center;
  }

  .player {
    width: 640px;
    height: 260px;
    text-align: center;
  }

  .logo {
    text-align: center;
    display: flex;
    justify-content: center;
    margin-top: 150px;
  }

  .logo img {
    height: 50vh;
  }

  h3 {
    color: #3363a4;
    font-size: 25px;
    text-align: center;
    font-family: Montserrat;
    font-weight: 700;
  }

  p {
    color: #fff;
    font-size: 9px;
    text-align: center;
    font-family: Montserrat;
    font-weight: 300;
  }
}
</style>

<script>
</script>