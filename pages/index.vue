<template>
  <div>
    <v-row
      align="center"
      justify="center"
      class="full-height"
    >
      <v-col
        cols="12"
        class="text-center"
      >
        <div class="headline-name">
          {{ title }}
        </div>
        <div class="subhead my-4">
          Software Developer
        </div>
        <v-btn
          v-for="link in links"
          :key="link.name"
          :href="link.url"
          target="_blank"
          class="mx-1"
          icon
          x-large
        >
          <v-icon x-large>
            {{ link.icon }}
          </v-icon>
        </v-btn>
      </v-col>
    </v-row>
  </div>
</template>

<script>
export default {
  data () {
    return {
      title: 'Austin Hedeen',
      links: [
        {
          name: 'LinkedIn',
          url: 'https://www.linkedin.com/in/austinhedeen',
          icon: 'mdi-linkedin-box',
        },
        {
          name: 'GitHub',
          url: 'https://github.com/Bejoty',
          icon: 'mdi-github-box',
        },
      ],
    }
  },
}
</script>

<style scoped>
  .headline-name {
    font-size: 3rem;
    font-family: Alegreya, serif;
  }

  .subhead {
    font-size: 1.5rem;
    font-family: Raleway, serif;
  }

  .full-height {
    height: calc(100vh - 24px);
  }
</style>
