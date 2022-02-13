<template>
  <v-app>
    <v-main>
      <router-view/>
    </v-main>
  </v-app>
</template>

<script>

export default {
  name: 'App',

  data: () => ({
    //
  }),
};
</script>

<style>
* {
  box-sizing : border-box;
}
#app {
  @import url('https://fonts.googleapis.com/css2?family=Baloo+Bhaijaan+2:wght@500&family=Darker+Grotesque&family=M+PLUS+1:wght@300&family=Merriweather+Sans&family=Noto+Sans+JP&family=Sawarabi+Gothic&display=swap');
  @import "./assets/stylesheet.css"
}
</style>