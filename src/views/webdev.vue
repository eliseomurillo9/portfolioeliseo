 <template>
  <v-parallax
    scale="1.4"
    height="90vh"
    class="responsive-portrait"
    src="/assets/img/union.jpg"
    ><div class="logo"><img src="/assets/img/logoem.png" alt="logo" /></div>
  </v-parallax>
  <v-parallax scale="1.3" dark src="/assets/img/backgroundrombos.jpg">
  <h2 class="about-title">Web Projects</h2>
    <v-row align="center" justify="center">
      <v-col class="text-center image-a box mt-xs-n7 mt-sm-n7 ml-sm-5 mr-sm-5 " cols="10">
        
        <v-img
          style="cursor: pointer"
          @click="goToWebsite('https://eliseomurillo9.github.io')"
          :src="imageSite"
        />
      </v-col>
    </v-row>
    <v-row align="center" justify="center">
      <v-col class="text-center box  ml-sm-5 mr-sm-5" cols="10">
        <h2 class="about-title">
          Projects done for FreeCodeCamp certification
        </h2>
        <iframe
          class="centerPen"
          scrolling="no"
          title="IKEA"
          src="https://codepen.io/eliseomurillo9/embed/XWaKYmP?default-tab=result&theme-id=dark"
          frameborder="no"
          loading="lazy"
          allowtransparency="true"
          allowfullscreen="true"
        >
          See the Pen
          <a href="https://codepen.io/eliseomurillo9/pen/XWaKYmP"> IKEA</a> by
          Josue (<a href="https://codepen.io/eliseomurillo9">@eliseomurillo9</a
          >) on <a href="https://codepen.io">CodePen</a>.
        </iframe>
      </v-col>
    </v-row>
    <v-row align="center" justify="center">
      <v-col class="text-center box mt-sm-n7 ml-sm-5 mr-sm-5 mb-10" cols="10">
        <iframe
          class="centerPen"
          scrolling="no"
          title="JS"
          src="https://codepen.io/eliseomurillo9/embed/QWMdEwq?default-tab=result&theme-id=dark"
          frameborder="no"
          loading="lazy"
          allowtransparency="true"
          allowfullscreen="true"
        >
          See the Pen
          <a href="https://codepen.io/eliseomurillo9/pen/QWMdEwq"> JS</a> by
          Josue (<a href="https://codepen.io/eliseomurillo9">@eliseomurillo9</a
          >) on <a href="https://codepen.io">CodePen</a>.
        </iframe>
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

.centerPen {
  height: 731px;
  width: 100%;
}

.image-a {
  height: 400px;
  transition-duration: 1s;
  transition-delay: 1s;
}

.about-title {
  font-size: 5rem;
  text-align: center;
  color: #3466aa;
  line-height: 1;
  font-family: Montserrat;
  font-weight: 600;
  margin-bottom: 50px;
  margin-top: 100px;
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
}
</style>

<script>
export default {
  data: () => ({
    mirror: true,
    imageSite: "/assets/img/siteweb.jpg",
  }),
  methods: {
    goToWebsite(site) {
      window.open(site, "_blank");
    },
  },
};
</script>
