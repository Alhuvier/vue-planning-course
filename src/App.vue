<template>
  <v-app>
    <v-app-bar app>
      <nav-bar />
    </v-app-bar>
    <v-main>
      <router-view />
    </v-main>
  </v-app>
</template>

<script lang="ts">
import Vue from 'vue'
import navBar from './components/navBar.vue'

export default Vue.extend({
  name: 'App',
  components: {
    navBar
  },
  data: () => ({
    //
  })
})
</script>
