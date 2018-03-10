<template>
<v-content>
  <section>
    <v-parallax :src="require('@/assets/title-hero.jpg')" height="450">
      <v-layout column align-center justify-center class="white--text">
        <h1 class="white--text mb-2 display-1 text-xs-center">Steven Avelino</h1>
        <div class="subheading mb-3 text-xs-center">Technicien en développement d'applications</div>
      </v-layout>
    </v-parallax>
  </section>
</v-content>
</template>

<script>
export default {
  name: 'Home',
  data () {
    return {
      title: 'Steven Avelino'
    }
  }
}
</script>


<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
