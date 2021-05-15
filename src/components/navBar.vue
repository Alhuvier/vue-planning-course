<template>
  <v-bottom-navigation v-model="value">
    <v-btn value="planning">
      <span>Planning</span>

      <v-icon>mdi-calendar</v-icon>
    </v-btn>

    <v-btn value="courses">
      <span>Courses</span>

      <v-icon>mdi-basket</v-icon>
    </v-btn>
  </v-bottom-navigation>
</template>

<script lang="ts">

export default {
  data: () :{value:string} => ({ value: 'planning' })
}

</script>
