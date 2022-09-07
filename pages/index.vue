<template>
  <div class="main">
    <v-tabs
      v-model="tab"
      centered
      icons-and-text
    >
      <v-tabs-slider></v-tabs-slider>

      <v-tab href="#tab-1" @click="componentName = 'home'">
        <p>{{ $t("home") }}</p>
        <v-icon>mdi-home-outline</v-icon>
      </v-tab>

      <v-tab href="#tab-2" @click="componentName = 'works'">
        <p>{{ $t("works") }}</p>
        <v-icon>mdi-briefcase-outline</v-icon>
      </v-tab>

      <v-tab href="#tab-3" @click="componentName = 'contact'">
        <p>{{ $t("contact") }}</p>
        <v-icon>mdi-human-greeting-proximity</v-icon>
      </v-tab>
    </v-tabs>

    <v-tabs-items v-model="tab">
      <v-tab-item v-for="i in 3" :key="i" :value="'tab-' + i">
        <component :is="componentName" />
      </v-tab-item>
    </v-tabs-items>
  </div>
</template>

<script>
import home from "../components/home/index.vue";
import works from "../components/works/index.vue"
import contact from "../components/contact/index.vue"
export default {
  name: "IndexPage",
  data() {
    return {
      tab: null,
      componentName: "home",
    };
  },
};
</script>
<style lang="scss" scoped>
.main {
  height: 100vh;
  font-family: 'Cinzel', serif;
}
</style>
