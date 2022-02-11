<template>
  <v-container fluid style="padding: 0">
    <v-row>
      <v-parallax
        scale="2"
        height="100vh"
        src="/assets/img/COVERnew.jpg"
      ></v-parallax>
    </v-row>
    <div class="bg planeanimation">
      <img class="plane" src="/assets/img/AirFigure.png" alt="airbus" />
      <v-row justify="start">
        <v-col
          cols="6"
          offset="6"
          align-self="center"
          class="mt-10 mr-90 ml-10 mb-n9"
          style="text-align: center"
        >
          <img
            src="/assets/img/aviation.png"
            atl="Aviation"
            width="300"
            class="bioImg"
          />
        </v-col>
      </v-row>
      <v-row justify="end">
        <v-col
          cols="6"
          align-self="center"
          class="mb-10 mr-10 mr-sm-15"
          style="text-align: center; "
        >
          <h2>Aviation</h2>
          <h4>2014 - 2020</h4>
        </v-col>
      </v-row>
      <v-row justify="start">
        <v-col
          cols="6"
          offset="6"
          align-self="center"
          class="mt-10 mr-10 ml-10 mb-n9"
          style="text-align: center"
        >
          <img
            src="/assets/img/production.png"
            atl="Aviation"
            width="300"
            class="bioImg"
          />
        </v-col>
      </v-row>
      <v-row justify="end">
        <v-col
          cols="6"
          offset="6"
          align-self="center"
          class="mr-10 ml-10"
          style="text-align: center"
        >
          <h2>Audiovisual</h2>
          <h4>2014 - 2020</h4>
        </v-col>
      </v-row>
      <v-row justify="start">
        <v-col
          cols="6"
          offset="6"
          align-self="center"
          class="mt-15 mr-10 ml-10 mb-n9"
          style="text-align: center"
        >
          <img
            src="/assets/img/web.png"
            atl="Aviation"
            width="520"
            class="bioImg"
          />
        </v-col>
      </v-row>
      <v-row justify="end">
        <v-col
          cols="8"
          align-self="start"
          class="mr-10 ml-12 mb-15"
          style="text-align: center"
        >
          <div class="respon">
            <h2>Web Development</h2>
          </div>
          <h4>2014 - 2020</h4>
        </v-col>
      </v-row>

      <v-row>
        <v-col class="ma-16" style="text-align: center">
          <h3 class="question">Want to know more about me?</h3>
          <v-btn
            rounded="lg"
            class="buttom-more"
            style="background-color: white"
            href="#about"
          >
            See more
          </v-btn>
        </v-col>
      </v-row>
    </div>
    <div class="bg-2">
      <h2 class="projectTitle" id="portfolio">Projects</h2>

      <v-row justify="center">
        <v-col
          class="mb-10 mt-15"
          align-self="center"
          xs="6"
          sm="3"
          md="3"
          lg="3"
        >
          <v-row justify="center">
            <v-card class="mx-auto, animation" href="#video" dark>
              <h3 class="textbox">Videos</h3>
            </v-card>
          </v-row>
        </v-col>
        <v-col
          class="mb-10 mt-15"
          align-self="center"
          xs="6"
          sm="3"
          md="3"
          lg="3"
        >
          <v-row justify="center">
            <v-card class="mx-auto, animation-gd" href="#desings" dark>
              <h3 class="textbox" s>Graphic Design</h3>
            </v-card>
          </v-row>
        </v-col>
        <v-col
          class="mb-10 mt-15"
          align-self="center"
          xs="6"
          sm="3"
          md="3"
          lg="3"
        >
          <v-row justify="center">
            <v-card class="mx-auto, animation-p" href="#photography" dark>
              <h3 class="textbox">Photography</h3>
            </v-card>
          </v-row>
        </v-col>
        <v-col
          class="mb-10 mt-15"
          align-self="center"
          xs="6"
          sm="3"
          md="3"
          lg="3"
        >
          <v-row justify="center">
            <v-card class="mx-auto, animation-wd" dark>
              <h3 class="textbox">
                Web<br />
                Development
              </h3>
            </v-card>
          </v-row>
        </v-col>
      </v-row>
    </div>
  </v-container>
</template>

<style scoped>
* {
  margin: 0%;
  padding: 0%;
}
h2 {
  font-size: 90px;
  text-align: center;
  color: #fff;
  line-height: 1;
  font-weight: 500;
  font-family: Montserrat;
  font-weight: 600;
}

h4 {
  color: #fff;
  font-weight: 100;
  font-size: 30px;
  text-align: center;
  font-family: Montserrat;
  font-weight: 200;
}

.bg {
  background-image: url("../../public/assets/img/background-2.jpg");
  background-size: cover;
}
.bg-2 {
  background-color: #1d1d1d;
}

.animation {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: row;
  color: #fff;
  border: solid;
  height: 175px;
  width: 300px;
  border-color: rgb(109, 106, 106, 0.4);
  border-radius: 15px;
  background: linear-gradient(#464646, #1d1d1d);
  transition: ease-in-out, 0.3s;
}

.animation:hover {
  background-image: url("../../public/assets/img/portada-video.gif");
  background-size: cover;
  border-color: #fff;
  cursor: pointer;
}

.animation-gd {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: row;
  color: #fff;
  border: solid;
  height: 175px;
  width: 300px;
  border-color: rgb(109, 106, 106, 0.4);
  border-radius: 15px;
  background: linear-gradient(#464646, #1d1d1d);
  transition: ease-in-out, 0.3s;
}

.animation-gd:hover {
  background-image: url("../../public/assets/img/portada-video.gif");
  background-size: cover;
  border-color: #fff;
  cursor: pointer;
}

.animation-p {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: row;
  color: #fff;
  border: solid;
  height: 175px;
  width: 300px;
  border-color: rgb(109, 106, 106, 0.4);
  border-radius: 15px;
  background: linear-gradient(#464646, #1d1d1d);
  transition: ease-in-out, 0.3s;
}

.animation-p:hover {
  background-image: url("../../public/assets/img/PHOTOS.gif");
  background-size: cover;
  border-color: #fff;
  cursor: pointer;
}

.animation-wd {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: row;
  color: #fff;
  border: solid;
  height: 175px;
  width: 300px;
  border-color: rgb(109, 106, 106, 0.4);
  border-radius: 15px;
  background: linear-gradient(#464646, #1d1d1d);
  transition: ease-in-out, 0.3s;
}

.animation-wd:hover {
  background-image: url("../../public/assets/img/coding.gif");
  background-size: cover;
  border-color: #fff;
  cursor: pointer;
}
.question {
  color: white;
  font-weight: bold;
  font-size: 70px;
}

.textbox {
  font-size: 3rem;
  text-align: center;
  line-height: 0.9;
}

.projectTitle {
  font-size: 90px;
  text-align: center;
  padding-top: 55px;
  color: #3363a4;
  font-family: Montserrat;
  font-weight: 700;
}

.bioImg {
  width: 22vw;
}

.planeanimation {
  position: relative;
  overflow: hidden;
}

.plane {
  height: 50vh;
  position: relative;
  left: 98%;
  top: 0%;
}

@media (max-width: 600px) {
  .respon {
    display: flex;
    justify-content: start;
    margin-left: 160px;
    width: 50px;
  }
}
@media (max-width: 900px) {
  h2 {
    font-size: 20px;
    text-align: end;
    color: #fff;
    line-height: 1;
  }

  h4 {
    color: #fff;
    font-weight: 100;
    font-size: 10px;
    text-align: end;
  }

  .bioImg {
    width: 150px;
  }

  .question {
    color: white;
    font-weight: bold;
    font-size: 30px;
  }
  .animation {
    height: 100px;
    width: 145px;
  }

  .textbox {
    font-size: 1.3rem;
    text-align: center;
  }

  .projectTitle {
    font-size: 90px;
    text-align: center;
    padding-top: 55px;
    padding-bottom: 55px;
    color: #3363a4;
  }

  .responsivepro {
    padding-bottom: 25px;
  }

  .plane {
    height: 20vh;
    position: relative;
    left: 98%;
    top: 0%;
  }
}
</style>


<script>
export default {
  data: () => ({
    scripts: [
      {
        src: "https://cdnjs.cloudflare.com/ajax/libs/ScrollMagic/2.0.8/ScrollMagic.min.js",
        integrity:
          "sha512-8E3KZoPoZCD+1dgfqhPbejQBnQfBXe8FuwL4z/c8sTrgeDMFEnoyTlH3obB4/fV+6Sg0a0XF+L/6xS4Xx1fUEg==",
      },
      {
        src: "https://cdnjs.cloudflare.com/ajax/libs/ScrollMagic/2.0.8/plugins/debug.addIndicators.min.js",
        integrity:
          "sha512-RvUydNGlqYJapy0t4AH8hDv/It+zKsv4wOQGb+iOnEfa6NnF2fzjXgRy+FDjSpMfC3sjokNUzsfYZaZ8QAwIxg==",
      },
      {
        src: "https://cdnjs.cloudflare.com/ajax/libs/ScrollMagic/2.0.8/plugins/animation.gsap.min.js",
        integrity:
          "sha512-5/OHwmQzDSBS0Ous4/hlYoWLHd06/d2r7LdKZQVBXOA6PvOqWVXtdboiLTU7lQTGyVoKVTNkwi0ol4gHGlw5ww==",
      },
      {
        src: "https://cdnjs.cloudflare.com/ajax/libs/gsap/2.1.2/TweenLite.min.js",
        integrity:
          "sha512-pvDW4tehKKsohH97164HwKwRGFpzayEFWTVbk8HuUoLIQ7Jp+WLN5XYokVuoCj2aT6dy8ihbW8SRTG1k0W4mSQ==",
      },
      {
        src: "https://cdnjs.cloudflare.com/ajax/libs/gsap/2.1.2/TimelineLite.min.js",
        integrity:
          "sha512-tSIDeirKC6suYILHqqPuZH3s0MvD4a5vCHXhBIcdmq4gQXZ2IB3fEYA5x2f3D2p/CbSqzKEvuTEVbS5VZ2u+ew==",
      },
      {
        src: "https://cdnjs.cloudflare.com/ajax/libs/gsap/2.1.2/plugins/CSSPlugin.min.js",
        integrity:
          "sha512-ocsFo48WU8Xq6Y1Lwi7psXRAujG9E4TKNR4q1DbrKzaaxOMTEoao/a+mDoB+cYzY4lwbyxvqjkp/ZA1/MNlfsg==",
      },
      {
        src: "https://cdnjs.cloudflare.com/ajax/libs/gsap/2.1.2/plugins/BezierPlugin.min.js",
        integrity:
          "sha512-plyexAULVlTExvDn2yUZFJV9F8q+53MC/GpU9dEuNGXmrrI3J8Rcffjvxg3OOBALBvF+UILPLIBEoCeF2maqTQ==",
      },
    ],
    scriptElements: [],
  }),
  async mounted() {
    await this.loadScripts();
    setTimeout(() => {
      this.initPlane();
    }, 1000);
  },
  methods: {
    async loadScripts() {
      for (const script of this.scripts) {
        let scriptElement = document.createElement("script");
        scriptElement.setAttribute("src", script.src);
        scriptElement.setAttribute("integrity", script.integrity);
        scriptElement.setAttribute("crossorigin", "anonymous");
        scriptElement.setAttribute("referrerpolicy", "no-referrer");

        this.scriptElements.push(scriptElement);
        await document.head.appendChild(scriptElement);
      }
    },
    initPlane() {
      const flightPath = {
        curviness: 1,
        autoRotate: true,
        values: [
          { x: -900, y: 900 },
          { x: -1000, y: 1100 },
          { x: -1100, y: 1200 },
          { x: -1300, y: 1300 },
          { x: -1800, y: 1500 },
          { x: -2000, y: 1600 },
          { x: -2300, y: window.innerWidth },
        ],
      };

      const tween = new TimelineLite();

      tween.add(
        TweenLite.to(".plane", 1, {
          bezier: flightPath,
          ease: Power1.easeInOut,
        })
      );
      const controller = new ScrollMagic.Controller();

      const scene = new ScrollMagic.Scene({
        triggerElement: ".planeanimation",
        duration: 3000,
        triggerHook: 1,
      })
        .setTween(tween)
        .addTo(controller);
    },
  },
};
</script>


<style>
</style>
