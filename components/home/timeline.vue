<template>
  <div class="d-flex flex-column align-center">
    <div class="timeline-title">Experience</div>
    <v-timeline id="timeline" dense clipped>
      <v-timeline-item
        v-for="(year, i) in years"
        :key="i"
        :color="year.color"
        small
      >
        <div class="py-4">
          <span
            :class="`headline font-weight-bold ${year.color}--text`"
            v-text="year.year"
          ></span>
          <div :class="` ${year.color}--text`">
            {{ year.title }}
          </div>
        </div>
      </v-timeline-item>
    </v-timeline>
  </div>
</template>
<script>
export default {
  data: () => ({
    years: [
      {
        color: "cyan",
        year: "2022-April / Now ",
        title: "Frontend Developer",
      },
      {
        color: "orange",
        year: "2021-December / 2022-April ",
        title: "QA Tester",
      },
      {
        color: "cyan",
        year: "2021-March / 2021-December ",
        title: "Frontend Tester",
      },
      {
        color: "orange",
        year: "2020-December / 2021-March ",
        title: "Software Support Specialist",
      },
    ],
  }),
};
</script>
<style lang="scss">
#timeline {
  margin-right: 50px;
}
.timeline-title {
  margin-top: 50px;
  margin-bottom: 30px;
  font-size: 35px;
  font-weight: 500;
  color: #D36B00;
}
</style>