 <template>
  
    <v-parallax
      scale="1.4"
      height="100vh"
      class="responsive-portrait"
      src="/assets/img/campamento.jpg"
      ><div class="logo"><img src="/assets/img/logoem.PNG" alt="logo" /></div>
      </v-parallax
    >
    <v-parallax
    scale="1.5"
    dark
    src="/assets/img/backgroundrombos.jpg"
  >
    <v-row align="center" justify="center">
      <v-col class="text-center box mt-12 ml-sm-5 mr-sm-5" cols="10">
        <div>
          <h2 class="about-title">About me</h2>
          <br />
          <p>
            Soy Eliseo Murillo, un joven Salvadoreño de 26 años, piloto y
            productor audiovisual. Actualmente resido en Francia, donde me estoy
            entrenando como web developer.
          </p>
          <br />

          <p>
            Inicie mis estudios en el año 2014 en “Escuela de Aviación Panal” en
            El Salvador, donde al cabo de cuatro años logré graduarme como
            piloto comercial. Posterior a ello, del año 2018 al 2020, me
            desempeñe como CFI dentro de la misma escuela.
          </p>
          <br />

          <p>
            Mientras me formaba como piloto, inició mi pasión por la producción
            y diseño. Realizando de forma autodidacta, cursos relacionados a la
            producción audiovisual, fotografía y softwares de diseño. Llevando
            así, a poder desempeñarme en el rubro como editor de video,
            asistente de producción, camarógrafo y dronista con diversas
            productoras, agencias y marcas comerciales, del año 2015 hasta la
            actualidad.
          </p>
          <br />

          <p>
            A consecuencia del COVID-19, decidí cambiar mi rumbo profesional y
            fusionar todas mis habilidades para desempeñarlas en la
            informática.<br />Actualmente, me encuentro realizando cursos que
            incluyen tecnologías tales como html, css y javascript, buscando el
            formarme como web developer
          </p>
          <br />

          <p>
            Mi meta es poder seguir desarrollándome como un programador full
            stack, donde pueda incluir mis habilidades y experiencias
            profesionales.
          </p>
        </div>
      </v-col>
    </v-row>
    <v-row align="center" justify="center">
      <v-col class="text-center box mt-12 mb-12 ml-sm-5 mr-sm-5" cols="10">
        <div class="cv" style="margin-bottom: 45px">
          <h2 style="text-align: center">Experiencia</h2>
          <h3>2014</h3>
          <v-divider
            inset
            thickness="2px"
            theme="dark"
            role="presentation"
          ></v-divider>
          <p>
            Camarografo, editor de video y dronista - Mediolleno Producciones,
            El Salvador.
          </p>
          <h3>2016 - 2018</h3>
          <v-divider
            inset
            thickness="2px"
            theme="dark"
            role="presentation"
          ></v-divider>
          <p>
            Freelance como dronista, camarógrafo, editor de video y asistente de
            producción - El Salvador.
          </p>
          <h3>2018 - 2019</h3>
          <v-divider
            inset
            thickness="2px"
            theme="dark"
            role="presentation"
          ></v-divider>
          <p>
            Director y productor de contenido - Iglesia COMPAZ, El Salvador.
          </p>
          <h3>2018 - 2020</h3>
          <v-divider
            inset
            thickness="2px"
            theme="dark"
            role="presentation"
          ></v-divider>
          <p>Instructor de vuelo - Escuela de Aviación PANAL, El Salvador.</p>
          <h3>2020 - Presente</h3>
          <v-divider
            inset
            thickness="2px"
            theme="dark"
            length="1105px"
            role="presentation"
          ></v-divider>
          <p>Freelance como diseñador, editor y animador - El Salvador</p>
        </div>
      </v-col>
    </v-row>
    <v-row align="center" justify="center">
      <v-col class="text-center box-soft mt-12 mb-12 ml-sm-5 mr-sm-5" cols="10">
        <div class="design">
          <h3>softwares</h3>
          <div class="softwarelogo">
            <img src="/assets/img/photoshop.PNG" alt="photoshop" />
            <img src="/assets/img/premier.PNG" alt="premier" />
            <img src="/assets/img/after.PNG" alt="after" />
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
            <img src="/assets/img/html.PNG" alt="html" />
            <img src="/assets/img/css.PNG" alt="html" />
            <img src="/assets/img/javascript.PNG" alt="html" />
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

.about-title{
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