<template>
  <v-bottom-navigation v-model="value">
    <v-btn value="home" to="/">
      <span>Home</span>
      <v-icon>mdi-home</v-icon>
    </v-btn>

    <v-btn value="planning" to="/planning">
      <span>Planning</span>
      <v-icon>mdi-calendar</v-icon>
    </v-btn>

    <v-btn value="courses" to="/courses">
      <span>Courses</span>
      <v-icon>mdi-basket</v-icon>
    </v-btn>

    <v-btn value="about" to="/about">
      <span>About</span>
      <v-icon>mdi-information-outline</v-icon>
    </v-btn>
  </v-bottom-navigation>
</template>

<script lang="ts">

export default {
  data: () :{value:string} => ({ value: 'planning' })
}

</script>
