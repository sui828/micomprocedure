<template>
  <v-carousel
    cycle
    height="70vh"
    hide-delimiter-background
    delimiter-icon="circle"
  >
    <template v-slot:prev="{ on, attrs }">
      <v-btn
        color="#3ad52a"
        v-bind="attrs"
        v-on="on"
      >
        <span class="material-icons">
          chevron_left
        </span>
      </v-btn>
    </template>
    <template v-slot:next="{ on, attrs }">
      <v-btn
        color="#3ad52a"
        v-bind="attrs"
        v-on="on"
      >
        <span class="material-icons">
          chevron_right
        </span>
      </v-btn>
    </template>
    <v-carousel-item
      v-for="(item,i) in items"
      :key="i"
      :src="item.src"
    ></v-carousel-item>
  </v-carousel>
</template>

<script>
  export default {
    data () {
      return {
        items: [
          {
            src: 'https://i.gyazo.com/f7fcfd7bde06d3b9cf9e924d48522836.png'
          },
          {
            src: 'https://i.gyazo.com/c1452655f19cea23132b8c4437889d9d.png'
          },
          {
            src: 'https://i.gyazo.com/ced962f50f392b01044b48618b5eaa0b.png'
          },
          {
            src: 'https://i.gyazo.com/cee29dba2f336a57c7dc18aab723a6a4.png'
          },
          {
            src: 'https://i.gyazo.com/59d42d5f5670d7812e7dd4a9d2188c70.png'
          }
        ]
      }
    }
  }
</script>

<style lang="scss">
v-carousel {
  carousel-controls-bg: rgba(0,0,0, .7);
  carousel-dot-bg: rgba(0,0,0, .7);
  carousel-dot-inactive-opacity: .5;
  carousel-dot-active-opacity: 1;
  carousel-dot-hover-opacity: .8;
}
</style>