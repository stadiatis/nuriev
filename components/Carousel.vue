<template>
  <v-carousel>
    <v-carousel-item v-for="(item,i) in items" :src="item.src" :key="i"></v-carousel-item>
  </v-carousel>
</template>

<script>
  export default {
    data () {
      return {
        items: [
          {
            src: '/static/foto47.png'
          },
           {
            src: '/static/foto51.png'
          }
        ]
      }
    }
  }
</script>