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


