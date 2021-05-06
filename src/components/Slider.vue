<template>
 <div lg="12" md="12" sm="12" cols="12">
    <v-carousel
      cycle
      height="600"
      hide-delimiter-background
      show-arrows-on-hover
    >
      <v-carousel-item
        v-for="(item,i) in items"
        :key="i"
        :src="item.src"
      >
      </v-carousel-item>

    </v-carousel>
  </div>
</template>
<script>
export default {
  name: "Slider",
  data() {
    return {
     
      slides: [
        'First',
        'Second',
        'Third',
        'Fourth',
        'Fifth',
      ],
       items: [
        {
           src: require("../assets/slider1.jpg"),
        },
        {
         src: require("../assets/slider2.jpg"),
        },
      ],
    };
  },

  

  

};
</script>

<style scoped>

</style>