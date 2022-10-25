<template>
  <v-app>
    <v-main>
      <HomeView/>
    </v-main>
  </v-app>
</template>

<script>
import HomeView from './sections/HomeView.vue'

export default {
  name: 'App',

  components: {
    HomeView,
  },

  data: () => ({
    //
  }),
}
</script>
