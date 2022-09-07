<template>
  <v-carousel cycle hide-delimiters class="mt-5 mb-15 container">
    <v-carousel-item
      v-for="(item, i) in items"
      :key="i"
      :src="require(`@/assets/images/${item.src}.png`)"
      class="carousel"
      :href="item.href"
      target="_blank"
    ></v-carousel-item>
  </v-carousel>
</template>

<script>
export default {
  data() {
    return {
      items: [
        {
          src: "hexa",
          href: "https://pipeline-hexaverse.herokuapp.com/",
        },
        {
          src: "yepas",
          href: "https://yepas.com/",
        },
        {
          src: "calik",
          href: "https://ahmetcalik.blackstudio.agency/",
        },
      ],
    };
  },
};
</script>

<style lang="scss">
#works > div.v-window.mt-5.mb-15.container.v-item-group.theme--dark.v-carousel {
  height: 550px !important;
}

// #works > div.v-window.mt-5.mb-15.container.works-carousel.v-item-group.theme--dark.v-carousel{
//    @media screen and (max-width: 600px) {
//      padding: 0px 0 100px 0 !important;
//   }
// }
</style>