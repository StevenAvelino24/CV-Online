<template>
<v-content>
  <section>
    <v-parallax :src="require('@/assets/title-hero.jpg')" height="450">
      <vue-particles color="#000000" linesColor="#000000"></vue-particles>
      <v-layout column align-center justify-center class="white--text">
        <h1 class="white--text mb-2 display-1 text-xs-center">Steven Avelino</h1>
        <div class="subheading mb-3 text-xs-center">Technicien en développement d'applications Web</div>
        <v-btn href="/portfolio" class="purple lighten-1">Visitez mon Portfolio</v-btn>
      </v-layout>
    </v-parallax>
  </section>
  <section>
    <v-layout column wrap align-center class="my-5">
      <v-flex xs12>
        <v-container grid-list-xl>
          <v-layout row wrap align-center justify-center>
            <v-flex xs12 md4>
              <v-card class="elevation-0 transparent">
                <v-card-text class="text-xs-center">
                  <v-icon x-large class="purple--text text--lighten-2">contacts</v-icon>
                </v-card-text>
                <v-card-title primary-title class="layout justify-center">
                  <div class="headline text-xs-center">Informations</div>
                </v-card-title>
                <v-card-text>
                  <v-list class="transparent">
                    <v-list-tile>
                      <v-list-tile-action>
                        <v-icon class="purple--text text--lighten-2">email</v-icon>
                      </v-list-tile-action>
                      <v-list-tile-content>
                        steven.avelino24@outlook.com
                      </v-list-tile-content>
                    </v-list-tile>
                    <v-list-tile>
                      <v-list-tile-action>
                        <v-icon class="purple--text text--lighten-2">place</v-icon>
                      </v-list-tile-action>
                      <v-list-tile-content>
                        Chemin des Petits Esserts 8, 1053 Cugy
                      </v-list-tile-content>
                    </v-list-tile>
                    <v-list-tile>
                      <v-list-tile-action>
                        <v-icon class="purple--text text--lighten-2">phone</v-icon>
                      </v-list-tile-action>
                      <v-list-tile-content>
                        +41791359475
                      </v-list-tile-content>
                    </v-list-tile>
                    <v-list-tile>
                      <v-list-tile-action>
                        <v-icon class="purple--text text--lighten-2">card_travel</v-icon>
                      </v-list-tile-action>
                      <v-list-tile-content>
                        Suisse
                      </v-list-tile-content>
                    </v-list-tile>
                    <v-list-tile>
                      <v-list-tile-action>
                        <v-icon class="purple--text text--lighten-2">cake</v-icon>
                      </v-list-tile-action>
                      <v-list-tile-content>
                        21 ans
                      </v-list-tile-content>
                    </v-list-tile>
                  </v-list>
                </v-card-text>
              </v-card>
            </v-flex>
            <v-flex xs12 md7 offset-md1>
              <v-card class="elevation-0 transparent">
                <v-card-text class="text-xs-center">
                  <v-icon x-large class="purple--text text--lighten-2">person</v-icon>
                </v-card-text>
                <v-card-title primary-title class="layout justify-center">
                  <div class="headline text-xs-center">About me</div>
                </v-card-title>
                <v-card-text class="text-xs-center">
                  Je suis un étudiant de 21 ans qui suit une formation de Technicien en développement d'applications Web au CPNV.
                  J'habite à 15 minutes de Lausanne.</br></br>
                  Je m'intéresse au développement et à la programmation depuis mon plus jeune âge, dû à mon père qui était déjà très intéressé
                  à tout ce qui touche l'informatique.
                  J'ai donc appris beaucoup de choses par moi-même et les ai raffinées en travaillant et en étant formé </br></br>
                  Après mon école obligatoire que j'ai fini en filiaire VSG, j'ai voulu trouver un apprentissage en tant qu'informaticien.
                  J'ai trouvé cet apprentissage chez Nagravision où j'ai appris tout type de choses liés à l'informatique et au monde du travail.
                  Après avoir travaillé pendant plus d'un an dans une équipe de développement, j'ai décidé de poursuivre mes études en tant que développeur. </br></br>
                  J'ai donc choisi le CPNV qui offrait ce que je voulais en terme de formation.
                </v-card-text>
              </v-card>
            </v-flex>
          </v-layout>
        </v-container>
      </v-flex>
    </v-layout>
  </section>
  <section>
    <v-parallax :src="require('@/assets/exp-pro.jpg')" height="350">
      <v-layout column align-center justify-center class="white--text">
        <h1 class="white--text mb-2 display-1 text-xs-center">Expériences professionnelles</h1>
      </v-layout>
    </v-parallax>
  </section>
  <section>
    <v-layout column wrap align-center class="my-5">
      <timeline timeline-theme="#004D40">
        <timeline-title><h3 class="white--text">Formations & Expériences</h3></timeline-title>
        <timeline-item><h4 class="white--text">Apprentissage Informaticien Nagravision SA (2012 - 2016)</h4></timeline-item>
        <timeline-item :hollow="true"><h4 class="white--text">Formation Technicien en développement Web (2017 - 2019)</h4></timeline-item>
      </timeline>
    </v-layout>
  </section>
  <section>
    <v-parallax :src="require('@/assets/exp-pro.jpg')" height="350">
      <v-layout column align-center justify-center class="white--text">
        <h1 class="white--text mb-2 display-1 text-xs-center">Technologies connues</h1>
      </v-layout>
    </v-parallax>
  </section>
  <section>
    <v-layout column wrap justify-center class="my-5">
      <v-flex xs12>
        <v-container grid-list-xl>
          <v-layout row wrap align-center>
            <v-flex xs12 md5>
              <v-card class="elevation-0 transparent">
                <v-card-title primary-title class="layout justify-center">
                  <div class="headline">Langages Web</div>
                </v-card-title>
              </v-card>
              <v-card-text>
                <v-list class="transparent">
                  <v-list-tile>
                    <v-list-tile-action>
                      <img :src="require('@/assets/html-32.png')">
                    </v-list-tile-action>
                    <v-list-tile-content>
                      <vue-progress v-model="progressHTML" color="#FF6D00" border-color="#303030"></vue-progress>
                    </v-list-tile-content>
                  </v-list-tile>
                  <v-list-tile>
                    <v-list-tile-action>
                      <img :src="require('@/assets/css-32.png')">
                    </v-list-tile-action>
                    <v-list-tile-content>
                      <vue-progress v-model="progressCSS" color="#01579B" border-color="#303030"></vue-progress>
                    </v-list-tile-content>
                  </v-list-tile>
                  <v-list-tile>
                    <v-list-tile-action>
                      <img :src="require('@/assets/javascript-log.png')">
                    </v-list-tile-action>
                    <v-list-tile-content>
                      <vue-progress v-model="progressJS" color="#F0DB4F" border-color="#303030"></vue-progress>
                    </v-list-tile-content>
                  </v-list-tile>
                  <v-list-tile>
                    <v-list-tile-action>
                      <img :src="require('@/assets/php-logo-32.png')">
                    </v-list-tile-action>
                    <v-list-tile-content>
                      <vue-progress v-model="progressPHP" color="#6181b6" border-color="#303030"></vue-progress>
                    </v-list-tile-content>
                  </v-list-tile>
                  <v-list-tile>
                    <v-list-tile-action>
                      <img :src="require('@/assets/laravel-32.png')">
                    </v-list-tile-action>
                    <v-list-tile-content>
                      <vue-progress v-model="progressLaravel" color="#F4511E" border-color="#303030"></vue-progress>
                    </v-list-tile-content>
                  </v-list-tile>
                  <v-list-tile>
                    <v-list-tile-action>
                      <img :src="require('@/assets/Ruby-On-Rails.png')">
                    </v-list-tile-action>
                    <v-list-tile-content>
                      <vue-progress v-model="progressRails" color="#C62828" border-color="#303030"></vue-progress>
                    </v-list-tile-content>
                  </v-list-tile>
                  <v-list-tile>
                    <v-list-tile-action>
                      <img :src="require('@/assets/Vue.png')">
                    </v-list-tile-action>
                    <v-list-tile-content>
                      <vue-progress v-model="progressVue" color="#41B883" border-color="#303030"></vue-progress>
                    </v-list-tile-content>
                  </v-list-tile>
                </v-list>
              </v-card-text>
            </v-flex>
            <v-flex xs12 md5 offset-md2>
              <v-card class="elevation-0 transparent">
                <v-card-title primary-title class="layout justify-center">
                  <div class="headline text-xs-center">Autres langages</div>
                </v-card-title>
              </v-card>
              <v-card-text>
                <v-list class="transparent">
                  <v-list-tile>
                    <v-list-tile-action>
                      <img :src="require('@/assets/cpp-logo.png')">
                    </v-list-tile-action>
                    <v-list-tile-content>
                      <vue-progress v-model="progressCPP" color="#004482" border-color="#303030"></vue-progress>
                    </v-list-tile-content>
                  </v-list-tile>
                  <v-list-tile>
                    <v-list-tile-action>
                      <img :src="require('@/assets/python-logo.png')">
                    </v-list-tile-action>
                    <v-list-tile-content>
                      <vue-progress v-model="progressPython" color="#FFCE3D" border-color="#303030"></vue-progress>
                    </v-list-tile-content>
                  </v-list-tile>
                  <v-list-tile>
                    <v-list-tile-action>
                      <img :src="require('@/assets/java-logo.png')">
                    </v-list-tile-action>
                    <v-list-tile-content>
                      <vue-progress v-model="progressJava" color="#E76F00" border-color="#303030"></vue-progress>
                    </v-list-tile-content>
                  </v-list-tile>
                  <v-list-tile>
                    <v-list-tile-action>
                      <img :src="require('@/assets/ruby-logo.png')">
                    </v-list-tile-action>
                    <v-list-tile-content>
                      <vue-progress v-model="progressRuby" color="#8B0E06" border-color="#303030"></vue-progress>
                    </v-list-tile-content>
                  </v-list-tile>
                  <v-list-tile>
                    <v-list-tile-action>
                      <img :src="require('@/assets/elixir-logo.png')">
                    </v-list-tile-action>
                    <v-list-tile-content>
                      <vue-progress v-model="progressElixir" color="#240339" border-color="#303030"></vue-progress>
                    </v-list-tile-content>
                  </v-list-tile>
                  <v-list-tile>
                    <v-list-tile-action>
                      <img :src="require('@/assets/mysql-logo.png')">
                    </v-list-tile-action>
                    <v-list-tile-content>
                      <vue-progress v-model="progressSQL" color="#4474CA" border-color="#303030"></vue-progress>
                    </v-list-tile-content>
                  </v-list-tile>
                </v-list>
              </v-card-text>
            </v-flex>
          </v-layout>
        </v-container>
      </v-flex>
    </v-layout>
  </section>
  <v-footer class="purple lighten-1">
    <v-layout row wrap align-center>
      <v-flex xs12>
        <div class="white--text ml-3">
          Made with
          <a class="white--text" href="https://vuejs.org/">Vue.JS</a>
          and
          <a class="white--text" href="https://vuetifyjs.com">Vuetify</a>
          by
          <a class="white--text" href="https://github.com/StevenAvelino24">Steven Avelino</a>
        </div>
      </v-flex>
    </v-layout>
  </v-footer>
</v-content>
</template>

<script>
import { Timeline, TimelineItem, TimelineTitle } from 'vue-cute-timeline'
import VueProgress from 'vue-progress-bar'

export default {
  name: 'Home',
  components: {
    Timeline,
    TimelineItem,
    TimelineTitle,
    VueProgress
  },
  data () {
    return {
      title: 'Steven Avelino',
      progressHTML: 0.9,
      progressCSS: 0.7,
      progressJS: 0.8,
      progressPHP: 0.85,
      progressLaravel: 0.7,
      progressRails: 0.4,
      progressVue: 0.65,
      progressCPP: 0.75,
      progressPython: 0.8,
      progressJava: 0.6,
      progressRuby: 0.7,
      progressElixir: 0.3,
      progressSQL: 0.75
    }
  }
}
</script>


<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  ul {
    list-style-type: none;
  }
  #particles-js {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 450px;
  }
  .about-me {
    text-align: justify;
  }
</style>
