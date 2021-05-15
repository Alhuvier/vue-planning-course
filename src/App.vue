<template>
  <v-app>
    <nav-bar />
    <router-view />
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
