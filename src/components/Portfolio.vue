<template>
  <v-content>
    <section>
      <v-parallax :src="require('@/assets/portfolio.jpg')" height="300">
      <v-layout column align-center justify-center class="black--text">
        <h1 class="black--text mb-2 display-1 text-xs-center">Portfolio</h1>
        <v-btn href="/" class="blue darken-1">Retour à l'accueil</v-btn>
      </v-layout>
      </v-parallax>
    </section>
    <section>
      <v-layout column wrap align-center class="my-3">
        <v-flex xs12>
          <v-container grid-list-xl>
            <v-layout row wrap align-center justify-center>
              <v-flex xs12 md4>
                <v-card class="elevation-2" height="100%-16px">
                  <v-card-title primary-title class="layout justify-center">
                    <div>
                      <h3 class="headline mb-0">CPNV - MyTech</h3>
                    </div>
                  </v-card-title>
                  <v-card-text>
                    <div>Laravel and Vue.Js Application to manage students for CPNV</div>
                  </v-card-text>
                  <v-card-actions class="layout justify-center">
                    <a target="_blank" href="https://github.com/CPNV-ES/Mytech"><v-btn flat color="blue">See the repo on Github</v-btn></a>
                  </v-card-actions>
                </v-card>
              </v-flex>
              <v-flex xs12 md4>
                <v-card class="elevation-2" height="100%-16px">
                  <v-card-title primary-title class="justify-center">
                    <div>
                      <h3 class="headline mb-0">Pyctures</h3>
                    </div>
                  </v-card-title>
                  <v-card-text>
                    <div>Python application to manage pictures</div>
                  </v-card-text>
                  <v-card-actions class="layout justify-center">
                    <a target="_blank" href="https://github.com/StevenAvelino/Pyctures"><v-btn flat color="blue">See the repo on Github</v-btn></a>
                  </v-card-actions>
                </v-card>
              </v-flex>
              <v-flex xs12 md4>
                <v-card height="100%-16px" class="elevation-2" v-for="repo in repos" :key="repo.name">
                  <v-card-title primary-title class="layout justify-center">
                    <div>
                      <h3 class="headline mb-0">{{ repo.name }}</h3>
                    </div>
                  </v-card-title>
                  <v-card-text>
                    <div>{{ repo.description }}</div>
                  </v-card-text>
                  <v-card-actions class="layout justify-center">
                    <a target="_blank" :href="repo.html_url"><v-btn flat color="blue">See the repo on Github</v-btn></a>
                  </v-card-actions>
                </v-card>
              </v-flex>
            </v-layout>
          </v-container>
        </v-flex>
      </v-layout>
    </section>
  </v-content>
</template>

<script>
import axios from 'axios'

function getRepos (success) {
  axios.get('https://api.github.com/users/StevenAvelino24/repos').then(response => {
    success(response.data)
  })
}
export default {
  name: 'portfolio',
  data () {
    return {
      repos: []
    }
  },
  beforeRouteEnter: (to, from, next) => {
    getRepos(function (data) {
      next(vm => vm.setRepos(data))
    })
  },
  methods: {
    setRepos (data) {
      this.repos = data
    }
  }
}
</script>

<style scoped>

</style>


