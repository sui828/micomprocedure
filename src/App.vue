<template>
  <v-app>
    <v-main>
      <router-view/>
      <button class="page-top" @click="scrollTop">
        <div><img src="./assets/common/iconmonstr-arrow-66.svg" class="uarr"></div>
        <div class="top-text">PageTop</div>
      </button>
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