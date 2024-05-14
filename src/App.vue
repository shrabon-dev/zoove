<template>
  <v-app>
    <v-main>
      <Home/>
    </v-main>
  </v-app>
</template>

<script>
import Home from './views/Home.vue'

export default {
  name: 'App',

  components: {
    Home,
  },

  data: () => ({
    //
  }),
}
</script>
<style>
  a{
    text-decoration: none;
  }
  ul li{
    list-style: none;
  }
  :root{
   --main:#1C2752;
   --sub:#7E7E7E;
   --yellow:#FFB342;
   --inter: "Inter", sans-serif;
   --mulish: "Mulish", sans-serif;
  }
</style>
