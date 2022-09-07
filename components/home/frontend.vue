<template>
  <div id="frontend" class="d-flex flex-column align-center">
    <div class="frontend-title">Frontend</div>
    <div class="d-flex mt-5 img-container">
      <v-tooltip bottom>
        <template v-slot:activator="{ on, attrs }">
          <img
            src="../../assets/images/sass.png"
            height="50px"
            alt=""
            v-bind="attrs"
            v-on="on"
          />
        </template>
        <span> SASS </span>
      </v-tooltip>
      <v-tooltip bottom>
        <template v-slot:activator="{ on, attrs }">
          <img
            src="../../assets/images/js.png"
            v-bind="attrs"
            v-on="on"
            height="50px"
            alt=""
          />
        </template>
        <span>Javascript</span>
      </v-tooltip>
      <v-tooltip bottom>
        <template v-slot:activator="{ on, attrs }">
          <img
            src="../../assets/images/vue.png"
            v-bind="attrs"
            v-on="on"
            height="50px"
            alt=""
          />
        </template>
        <span>VueJS</span>
      </v-tooltip>
      <v-tooltip bottom>
        <template v-slot:activator="{ on, attrs }">
          <img
            src="../../assets/images/nuxt.png"
            v-bind="attrs"
            v-on="on"
            height="50px"
            alt=""
          />
        </template>
        <span>NuxtJS</span>
      </v-tooltip>

      <v-tooltip bottom>
        <template v-slot:activator="{ on, attrs }">
          <img
            src="../../assets/images/boostrap-vue.png"
            v-bind="attrs"
            v-on="on"
            height="50px"
            alt=""
          />
        </template>
        <span>Bootstrap Vue</span>
      </v-tooltip>
      <v-tooltip bottom>
        <template v-slot:activator="{ on, attrs }">
          <img
            src="../../assets/images/bootstrap.png"
            v-bind="attrs"
            v-on="on"
            height="50px"
            alt=""
          />
        </template>
        <span>Bootstrap</span>
      </v-tooltip>
      <v-tooltip bottom>
        <template v-slot:activator="{ on, attrs }">
          <img
            src="../../assets/images/vuetify.png"
            v-bind="attrs"
            v-on="on"
            height="50px"
            alt=""
          />
        </template>
        <span>Vuetify</span>
      </v-tooltip>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss">
#frontend {
  .frontend-title {
    font-size: 35px;
    margin-top: 50px;
    font-weight: 500;
      color: #D36B00;
  }
  .img-container {
    margin-top: 50px !important;
    img {
      margin-right: 5px;
    }
  }
}
</style>