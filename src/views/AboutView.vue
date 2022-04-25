 <template>
  <v-parallax
    scale="1.4"
    height="100vh"
    class="responsive-portrait"
    src="/assets/img/campamento.jpg"
    ><div class="logo"><img src="/assets/img/logoem.png" alt="logo" /></div>
  </v-parallax>
  <v-parallax scale="1.3" dark src="/assets/img/backgroundrombos.jpg">
    <v-row align="center" justify="center">
      <v-col class="text-center box mt-12 ml-sm-5 mr-sm-5" cols="10">
        <div>
          <h2 class="about-title">About me</h2>
          <br />
          <p>
            I am Eliseo Murillo, Salvadorian, 26 years old. Licensed pilot, and
            audiovisual producer. Currently, I am living in France, and training
            to be a web developer.
          </p>
          <br />

          <p>
            I started my certifications back in 2014 at “Escuela de Aviación
            Panal” in El Salvador, finishing in 2018, certified with a
            Commercial Pilot License and multi-engine and instructor rating.
            Once I acquired my licenses, I performed for two years as a
            certified flight instructor.
          </p>
          <br />

          <p>
            While I was studying to get my flight certification, I found passion
            on audiovisual production and graphic designing, I started
            self-paced courses related to audiovisual production, photography,
            and graphic designing. To the extend to gain experience in the area
            as video editor, production assistant, cameraman, photographer and
            drone operator for different producing and marketing agencies, and
            marketing brands.
          </p>
          <br />

          <p>
            Due to COVID-19 pandemic, I decided to expand my professional career
            combining all my skills into information technology area, with my
            versatility, autonomy and critical thinking. Currently I am coursing
            certifications including programming languages as html, css,
            javascrpit, as web developer.
          </p>
          <br />

          <p>
            My goal is to continue learning to perform as a full stack
            programmer, combining my skills and work experience.
          </p>
        </div>
      </v-col>
    </v-row>
    <v-row align="center" justify="center">
      <v-col class="text-center box mt-12 mb-12 ml-sm-5 mr-sm-5" cols="10">
        <div class="cv" style="margin-bottom: 45px">
          <h2 style="text-align: center">Experience</h2>
          <h3>2020 - Present</h3>
          <v-divider
            inset
            thickness="2px"
            theme="dark"
            role="presentation"
          ></v-divider>
          <p>Freelance as Graphic Designer, Video Editor and Animation - El Salvador</p>
          <h3>2018 - 2020</h3>
          <v-divider
            inset
            thickness="2px"
            theme="dark"
            role="presentation"
          ></v-divider>
          <p>certified Flight Instructor - Escuela de Aviación PANAL, El Salvador.</p>
          <h3>2018 - 2019</h3>
          <v-divider
            inset
            thickness="2px"
            theme="dark"
            role="presentation"
          ></v-divider>
          <p>
            Director and Content Producer - Iglesia COMPAZ, El Salvador.
          </p>
          <h3>2014</h3>
          <v-divider
            inset
            thickness="2px"
            theme="dark"
            role="presentation"
          ></v-divider>
          <p>
            Cameraman, video editor y drone operator - Mediolleno Producciones,
            El Salvador.
          </p>
        </div>
      </v-col>
    </v-row>
    <v-row align="center" justify="center">
      <v-col class="text-center box-soft mt-12 mb-12 ml-sm-5 mr-sm-5" cols="10">
        <div class="design">
          <h3>Softwares</h3>
          <div class="softwarelogo">
            <img src="/assets/img/photoshop.png" alt="photoshop" />
            <img src="/assets/img/premier.png" alt="premier" />
            <img src="/assets/img/after.png" alt="after" />
          </div>
        </div>
        <v-divider
          inset
          thickness="2px"
          theme="dark"
          role="presentation"
          vertical="90px"
        ></v-divider>
        <div class="webdev">
          <h3>Lenguajes</h3>
          <div class="softwarelogo">
            <img src="/assets/img/html.png" alt="html" />
            <img src="/assets/img/css.png" alt="html" />
            <img src="/assets/img/javascript.png" alt="html" />
          </div>
        </div>
      </v-col>
    </v-row>
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
.box {
  background-color: #363636;
  display: flex;
  flex-direction: column;
  border-radius: 15px;
  box-shadow: 0.3rem 0.3rem 1rem rgb(24 24 24 / 30%);
}

p {
  color: white;
}

h2 {
  color: #3466aa;
  font-size: 3rem;
}

.cv {
  text-align: center;
}

.cv h3 {
  margin-top: 45px;
  color: white;
  font-size: 25px;
}
.cv p {
  margin-top: 10px;
}

.box-soft {
  background-color: #363636;
  display: flex;
  flex-direction: row;
  justify-content: center;
  border-radius: 15px;
  box-shadow: 0.3rem 0.3rem 1rem rgb(24 24 24 / 30%);
}

.design {
  margin-right: 105px;
}

.design h3 {
  font-size: 25px;
}

.softwarelogo img {
  height: 75px;
  margin: 15px;
}

.webdev {
  margin-left: 105px;
}
.webdev h3 {
  font-size: 25px;
}

.about-title {
  font-size: 5rem;
  text-align: center;
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

  .about-title {
    font-size: 2rem;
  }
  .responsive-portrait {
    height: 10px;
  }

  .webdev {
    margin-left: 0px;
  }

  .design {
    margin-right: 0px;
  }

  .softwarelogo img {
    height: 45px;
    margin: 15px;
  }
}
</style>
<script>
export default {
  data: () => ({
    mirror: true,
  }),
};
</script>