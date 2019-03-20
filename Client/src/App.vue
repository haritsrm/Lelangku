<template>
  <div id="app">
    <v-card
    class="pa-3"
    flat
    height="300px"
    img="https://image.myanimelist.net/ui/5LYzTBVoS196gvYvw3zjwBjXr1IaXf2-Py4fXUuJgWg"
    >
      <v-toolbar
        dense
        floating
      >
        <v-text-field
          hide-details
          append-icon="search"
          single-line
          placeholder="Mau cari figure apa?"
        ></v-text-field>
      </v-toolbar>
    </v-card>
    <HelloWorld msg="Welcome to Your Vue.js App"/>
    <br>
    <v-container>
      <Workflow></Workflow>
    </v-container>
    <v-footer
    dark
    height="auto"
  >
    <v-card
      class="flex"
      flat
      tile
    >
      <v-card-title class="teal">
        <strong class="subheading">Get connected with us on social networks!</strong>

        <v-spacer></v-spacer>

        <v-btn
          v-for="icon in icons"
          :key="icon"
          class="mx-3"
          dark
          icon
        >
          <v-icon size="24px">{{ icon }}</v-icon>
        </v-btn>
      </v-card-title>

      <v-card-actions class="grey darken-3 justify-center">
        &copy;2018 — <strong>Vuetify</strong>
      </v-card-actions>
    </v-card>
  </v-footer>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import Workflow from './components/Workflow.vue'

export default {
  data(){
    return {
      icons: [
        'fab fa-facebook',
        'fab fa-twitter',
        'fab fa-google-plus',
        'fab fa-linkedin',
        'fab fa-instagram'
      ]
    }
  },
  name: 'app',
  components: {
    HelloWorld, Workflow
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
