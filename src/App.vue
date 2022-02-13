<template>
  <v-app>
    <v-main>
      <router-view/>
      <button class="page-top" @click="scrollTop"></button>
    </v-main>
  </v-app>
</template>

<script>

export default {
  name: 'App',
  methods: {
    scrollTop: function(){
      window.scrollTo({
        top: 0,
        behavior: "smooth"
      });
    }
  },
  data: () => ({
    //
  }),
};
</script>

<style>
* {
  box-sizing : border-box;
}
</style>