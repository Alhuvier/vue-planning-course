
<template>
  <v-bottom-navigation v-model='value' :background-color='color' grow app>
    <v-btn value='home' to='/' color='blue-grey'>
      <span>Home</span>
      <v-icon>mdi-home</v-icon>
    </v-btn>

    <v-btn value='planning' to='/planning' color='teal'>
      <span>Planning</span>
      <v-icon>mdi-calendar</v-icon>
    </v-btn>

    <v-btn value='courses' to='/courses' color='brown'>
      <span>Courses</span>
      <v-icon>mdi-basket</v-icon>
    </v-btn>

    <v-btn value='about' to='/about' color='indigo'>
      <span>About</span>
      <v-icon>mdi-information-outline</v-icon>
    </v-btn>
  </v-bottom-navigation>
</template>
<style lang='scss'>
#app .v-bottom-navigation .v-btn {
  height: inherit !important;
}
</style>

<script lang='ts'>
// TO FIX : Color background problem
export default {
  data: () :{value:string} => ({ value: 'planning' }),
  computed: {
    // eslint-disable-next-line @typescript-eslint/explicit-module-boundary-types
    color () {
      switch (this.value) {
        case 'home': return 'blue-grey'
        case 'planning': return 'teal'
        case 'courses': return 'brown'
        case 'about': return 'indigo'
        default: return 'blue-grey'
      }
    }
  }
}

</script>
