<template>
  <div id="works" class="container">
    <carousel class="works-carousel" />
    <works-list class="works-list" />
    <v-expansion-panels class="works-panels">
      <v-expansion-panel>
        <v-expansion-panel-header class="item">
          PURE CSS EXAMPLES
           <template v-slot:actions>
            <v-icon >
              $expand
            </v-icon>
          </template>
        </v-expansion-panel-header>
        <v-expansion-panel-content>
          <work-menu />
          <remake />
          <curs />
          <infinite />
        </v-expansion-panel-content>
      </v-expansion-panel>
    </v-expansion-panels>

    <portfolio-footer />
  </div>
</template>

<script>
import profil from "../home/profil.vue";
import PortfolioFooter from "../portfolioFooter.vue";
import Carousel from "./carousel.vue";
import Curs from "./curs.vue";
import Infinite from "./infinite.vue";
import Remake from "./remake.vue";
import WorkMenu from "./workMenu.vue";
import WorksList from "./worksList.vue";
export default {
  components: {
    profil,
    Carousel,
    WorkMenu,
    Remake,
    WorksList,
    Curs,
    Infinite,
    PortfolioFooter,
  },
};
</script>

<style lang="scss">
#works {
  min-height: 100vh;
  .works-carousel{
    animation: up 1s;
  }
   .works-list{
    animation: up 1.5s;
  }
   .works-panels{
    animation: down 2s;
  }
.item{
  font-size: 28px;
}
}
@keyframes up {
  from {
    transform: translateY(-100vw);
  }
  to {
    transform: translateY(0px);
  }
}
@keyframes down {
  from {
    transform: translateY(100vw);
  }
  to {
    transform: translateY(0px);
  }
}

</style>