<template>
  <v-app dark>
    <v-content>
      <v-container :fluid="fluidContainer">
        <nuxt />
      </v-container>
    </v-content>
  </v-app>
</template>

<script>
export default {
  data () {
    return {
      fluidContainer: true,
    }
  },
}
</script>
