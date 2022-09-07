<template>
  <div id="descriptions">
    <div class="name">Mücahit Kalabalık</div>
    <div class="title">Front-End Developer</div>
    <div class="contacts">
      <div class="github">
        <v-icon>mdi-github</v-icon>
        <a href="https://github.com/mucahitkalabalik" target="_blank">Github</a>
      </div>
      <div class="email">
        <v-icon class="email-icon"> mdi-card-account-mail-outline </v-icon>
        <a href="mailto:mucahitkalabalik@outlook.com"
          >mucahitkalabalik@outlook.com</a
        >
      </div>
      <div class="location">
        <v-icon>mdi-map-marker-circle</v-icon>
        <a
          target="_blank"
          href="https://www.google.com/maps/place/%C3%9Cmraniye%2F%C4%B0stanbul/@41.027176,29.0024447,12z/data=!3m1!4b1!4m5!3m4!1s0x14cac92b2df797b9:0xabff48934920c04a!8m2!3d41.0182327!4d29.1274334"
          >İstanbul - Turkey</a
        >
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss">
#descriptions {
  margin-top: 50px;
    @media screen and (max-width: $medium) {
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
  }
  .name {
    display: inline;
    font-size: 46px;
    letter-spacing: 5px;
      @media screen and (max-width: $medium) {
        text-align: center;
      }
  }
  .contacts {
    font-size: 14px !important;
    display: flex;
    align-items: column;
    justify-content: center;
    flex-direction: column;
  }
}
</style>