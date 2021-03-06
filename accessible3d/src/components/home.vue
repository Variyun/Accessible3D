<template>
    <v-container class="pa-0 ma-0" fluid> 
        <v-main class="pt-0" >
        <section id="hero">
        <v-row no-gutters>
            <v-img
                :min-height="'calc(100vh - ' + $vuetify.application.top + 'px)'"
                src="../assets/background.png"
            >
                <v-theme-provider dark>
                <v-container fill-height>
                    <v-row
                    align="center"
                    class="white--text mx-0"
                    justify="center"
                    >
                    <v-col
                        class="white--text text-center"
                        cols="12"
                        tag="h1"
                    >
                        <span
                        :class="[$vuetify.breakpoint.smAndDown ? 'display-1' : 'display-2']"
                        class="font-weight-light"
                        data-aos="fade-up" data-aos-duration="3000"
                        >
                        WELCOME TO
                        </span>

                        <br>

                        <span
                        :class="[$vuetify.breakpoint.smAndDown ? 'display-3': 'display-4']"
                        class="font-weight-black"
                        data-aos="zoom-in" data-aos-duration="3000" data-aos-delay="800"
                        >
                        ACCESSIBLE 3D
                        </span>
                    </v-col>

                    <v-scale-transition>
                        <v-btn
                            v-show="load"
                            class="align-self-end"
                            fab
                            outlined
                            @click="$vuetify.goTo('#about-us')"
                        >
                            <v-icon>mdi-chevron-double-down</v-icon>
                        </v-btn>
                    </v-scale-transition>
                    </v-row>
                </v-container>
                </v-theme-provider>
            </v-img>
            </v-row>
        </section>

        <section id="about-us">
            <div class="py-12"></div>

            <v-container class="text-center">
            <h2 class="display-2 font-weight-bold mb-3" data-aos="fade-up" data-aos-duration="500" data-aos-delay="100">
            ABOUT US
            </h2>

            <v-responsive
                class="mx-auto mb-8"
                width="56"
            >
                <v-divider class="mb-1"></v-divider>

                <v-divider></v-divider>
            </v-responsive>

            <v-responsive
                class="mx-auto title font-weight-light mb-8"
                max-width="720"
                data-aos="fade-down" data-aos-duration="500" data-aos-delay="200"
            >
               First and foremost, thank you for visiting our website! We are a team of dedicated geomatics engineers from the University of Calgary. As geomatics engineers, we strive to bring more awareness about the awesome technology we learn about and use in our ever-growing industry through ACCESSIBLE 3D. From each of us on the team, we hope that you can find everything you need to dive into the world of 3D modelling! 
            </v-responsive>
            
            <v-row >
                <v-col data-aos="fade-down" data-aos-delay="300" data-aos-duration="1000">
                    <v-avatar
                        class="elevation-12 mb-3"
                        size="128"
                    >
                        <v-img src="../assets/aa_icon.png"></v-img>
                    </v-avatar>
                    <br/>
                    <span>AARON</span>
                </v-col>
                <v-col data-aos="fade-down" data-aos-delay="400" data-aos-duration="1000">
                    <v-avatar
                        class="elevation-12 mb-3"
                        size="128"
                    >
                        <v-img src="../assets/jh_icon.png"></v-img>
                    </v-avatar>
                    <br/>
                    <span>JOSH</span>
                </v-col>
                <v-col data-aos="fade-down" data-aos-delay="500" data-aos-duration="1000">
                    <v-avatar
                        class="elevation-12 mb-3"
                        size="128"
                    >
                        <v-img src="../assets/mk_icon.png"></v-img>
                    </v-avatar>
                    <br/>
                    <span>MICHAEL</span>
                </v-col>
                <v-col data-aos="fade-down" data-aos-delay="600" data-aos-duration="1000">
                    <v-avatar
                        class="elevation-12 mb-3"
                        size="128"
                    >
                        <v-img src="../assets/wy_icon.png"></v-img>
                    </v-avatar>
                    <br/>
                    <span>WYNAND</span>
                </v-col>
            </v-row>
            <v-row align="center" justify="center">
                <v-scale-transition>
                    <v-btn
                        v-show="load"
                        class="align-self-end"
                        fab
                        outlined
                        @click="$vuetify.goTo('#features')"
                    >
                        <v-icon>mdi-chevron-double-down</v-icon>
                    </v-btn>
                </v-scale-transition>
            </v-row>
            
            <div></div>
            </v-container>

            <div class="py-12"></div>
        </section>

        <section
            id="features"
        >
            <div class="py-12"></div>

            <v-container class="text-center">
            <h2 class="display-2 font-weight-bold mb-3" data-aos="fade-up" data-aos-duration="500" data-aos-delay="100">
            WHAT IS ACCESSIBLE 3D?
            </h2>

            <v-responsive
                class="mx-auto mb-12"
                width="56"
            >
                <v-divider class="mb-1"></v-divider>

                <v-divider></v-divider>
            </v-responsive>

            <v-row class="pb-10 mx-15" no-gutters> 
                <v-col class="px-0" align="left" justify="center">
                    <h3 class="font-weight-light" data-aos="fade-right" data-aos-duration="1800" data-aos-delay="500">
                    ACCESSIBLE 3D is about enabling everyday people to produce high quality 3D models using just a mobile phone camera, with no prior knowledge necessary. By making reconstruction accessible to all, the group aims to bring attention to the industry’s recent advancements in efficiency and cost.
                    </h3>
                    <p></p>
                    <h3 class="font-weight-light" data-aos="fade-right" data-aos-duration="1800" data-aos-delay="500"> 
                    Many of today’s hottest technologies (e.g. Computer vision, AI, Autonomy) require 3D data, whether it’s LIDAR, positioning, or model data. We hope to reduce the entry barrier for photogrammetry through education, in turn promotes innovation in engineering in the future.
                    </h3>
                </v-col>
                <v-col align="right" justify="center" class="hidden-md-and-down" cols="6">
                    <v-img src="../assets/phone_white.png" 
                    max-width="40%" 
                    :max-height="'calc(60vh)'" 
                    data-aos="fade-left"
                    data-aos-duration="2000"
                    data-aos-delay="500"> 
                    </v-img>
                </v-col> 
            </v-row>
              <v-row align="center" justify="center">
                <v-scale-transition>
                    <v-btn
                        v-show="load"
                        class="align-self-end"
                        fab
                        outlined
                        @click="$vuetify.goTo('#contact')"
                    >
                        <v-icon>mdi-chevron-double-down</v-icon>
                    </v-btn>
                </v-scale-transition>
            </v-row>
            </v-container>
            <div class="py-12"></div>
        </section>

        <v-sheet
            id="contact"
            color="#333333"
            dark
            tag="section"
            tile
        >
            <div class="py-12"></div>

            <v-container>
            <h2 class="display-2 font-weight-bold mb-3 text-uppercase text-center">Contact Us</h2>

            <v-responsive
                class="mx-auto mb-12"
                width="56"
            >
                <v-divider class="mb-1"></v-divider>

                <v-divider></v-divider>
            </v-responsive>

            <v-theme-provider light>
                <v-row>
                <v-col cols="12">
                    <v-text-field
                    flat
                    label="Name*"
                    solo
                    ></v-text-field>
                </v-col>

                <v-col cols="12">
                    <v-text-field
                    flat
                    label="Email*"
                    solo
                    ></v-text-field>
                </v-col>

                <v-col cols="12">
                    <v-text-field
                    flat
                    label="Subject*"
                    solo
                    ></v-text-field>
                </v-col>

                <v-col cols="12">
                    <v-textarea
                    flat
                    label="Message*"
                    solo
                    ></v-textarea>
                </v-col>

                <v-col
                    class="mx-auto"
                    cols="auto"
                >
                    <v-btn
                    color="indigo lighten-1"
                    x-large
                    >
                    Submit
                    </v-btn>
                </v-col>
                </v-row>
            </v-theme-provider>
            </v-container>

            <div class="py-12"></div>
        </v-sheet>
        </v-main>
        <v-fab-transition>
        <v-btn
            v-scroll="onScroll"
            v-show="fab"
            elevation="0"
            large
            fab
            fixed
            bottom
            right
            color="primary"
            @click="toTop"
        >
            <v-icon>mdi-chevron-double-up</v-icon>
        </v-btn>
        </v-fab-transition>
    </v-container> 
</template>

<style scoped>

</style>

<script>
  //Animation Library
  import AOS from 'aos';
  import 'aos/dist/aos.css';
  AOS.init();

  export default {
    name: 'home',
    methods: {
      onScroll (e) {
        if (typeof window === 'undefined') return
        const top = window.pageYOffset ||   e.target.scrollTop || 0
        this.fab = top > 20
      },
      toTop() {
        this.$vuetify.goTo(0)
      }
    },
    mounted() {
      this.load = true;  
      window.scrollTo(0, 0);
    },
    data: () => ({
        fab:false,
        load:false,
    }),
  }
</script>