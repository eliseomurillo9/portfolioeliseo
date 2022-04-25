 <template>
  <v-parallax
    scale="1.4"
    height="90vh"
    class="responsive-portrait"
    src="/assets/img/union.jpg"
    ><div class="logo"><img src="/assets/img/logoem.png" alt="logo" /></div>
  </v-parallax>
  <v-parallax scale="1.3" dark src="/assets/img/backgroundrombos.jpg">
    <div>
      <div class="title">
        <h2>Projects</h2>
      </div>
      <div class="cards">
        <div>
        <v-card class="card">
          <v-img src="/assets/img/enterprisephone.jpg" height="200px" cover></v-img>
          <v-card-title style="color: #3363a4">
            Company
          </v-card-title>

          <v-card-actions>
            <v-btn
              color="black-lighten-2"
              variant="text"
              @click="goToWebsite('https://eliseomurillo9.github.io')"
            >
              See site
            </v-btn>

            <v-spacer></v-spacer>

            <v-btn
              :icon="show ? 'mdi-chevron-up' : 'mdi-chevron-down'"
              @click="show = !show"
            ></v-btn>
          </v-card-actions>

          <v-expand-transition>
            <div v-show="show">
              <v-divider></v-divider>
              <v-card-title style="color: #3363a4">Languages</v-card-title>
              <v-card class="logos">
                <img src="/assets/img/732212.png" />
                <img src="/assets/img/Devicon-css3-plain.png" />
                <img src="/assets/img/600px-JavaScript-logo.png" />
              </v-card>
            </div>
          </v-expand-transition>
        </v-card>
        </div>
        <div>
        <v-card class="card">
          <v-img src="/assets/img/homeandgardenphone.jpg" height="200px" cover></v-img>

          <v-card-title style="color: #3363a4">
            Home & Garden
          </v-card-title>

          <v-card-actions>
            <v-btn
              color="black-lighten-2"
              variant="text"
              @click="goToWebsite('https://homegarden-pgaxg.ondigitalocean.app')"
            >
              See site
            </v-btn>

            <v-spacer></v-spacer>

            <v-btn
              :icon="show1 ? 'mdi-chevron-up' : 'mdi-chevron-down'"
              @click="show1 = !show1"
            ></v-btn>
          </v-card-actions>

          <v-expand-transition>
            <div v-show="show1">
              <v-divider></v-divider>
              <v-card-title style="color: #3363a4">Languages</v-card-title>
              <v-card class="logos">
                <img src="/assets/img/732212.png" />
                <img src="/assets/img/Devicon-css3-plain.png" />
                <img src="/assets/img/600px-JavaScript-logo.png" />
              </v-card>
            </div>
          </v-expand-transition>
        </v-card>
      </div>
    </div>
    
    </div>
  </v-parallax>
</template>
<style scoped>
.logo {
  text-align: center;
}

.logo img {
  height: 75vh;

  margin-top: 7%;
}

.title{
  display: flex;
  flex-direction: column;
  justify-content: center;
}

.title h2{
  font-size: 35px;
  color: #3466aa;
  text-align: center;
  margin: 25px 0 25px 0;
  font-family: Montserrat;
}

.cards {
  display: flex;
  flex-direction: row;
  justify-content: space-evenly;
}

.logos {
  display: flex;
  flex-direction: row;
  justify-content: center;
}

.logos img {
  height: 50px;
  margin: 15px;
  filter: drop-shadow(2px 3px 2px #4b4b4d);

  cursor: pointer;
  transition: 0.3s ease-in-out;
}

.logos img:hover {
  transform: scale(1.3);
  filter: drop-shadow(3px 4px 3px #4b4b4d, 20%);
}

.card {
  width: 404px;
  padding: 0%;
  margin: 0%;
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

  .centerPen {
    height: 400px;
    width: 100%;
  }
  .image-a {
    height: 200px;
  }
  .about-title {
    font-size: 20px;
    text-align: center;
    margin-bottom: 10px;
    margin-top: 10px;
  }

  .cards{
    display: flex;
    flex-direction: column;
    justify-content: center;  
    align-items: center;
  }

  .card {
  width: 204px;
  padding: 0%;
  margin-top: 15px;
}

.logos img {
  height: 40px;
}
}
</style>

<script>
export default {
  data: () => ({
    mirror: true,
    imageSite: "/assets/img/siteweb.jpg",
    show: false,
    show1: false,
  }),
  methods: {
    goToWebsite(site) {
      window.open(site, "_blank");
    },
  },
};
</script>
