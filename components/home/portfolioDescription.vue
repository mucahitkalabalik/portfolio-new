<template>
  <section id="portfolio-description">
    <div class="portfolio-title">Hola , Good Day !</div>
    <div class="portfolio-desc">
      Lorem Ipsum is simply dummy text of the printing and typesetting industry.
      Lorem Ipsum has been the industry's standard dummy text ever since the
      1500s, when an unknown printer took a galley of type and scrambled it to
      make a type specimen book. It has survived not only five centuries, but
      also the leap into electronic typesetting, remaining essentially
      unchanged. It was popularised in the 1960s with the release of Letraset
      sheets containing Lorem Ipsum passages, and more recently with desktop
      publishing software like Aldus PageMaker including versions of Lorem
      Ipsum.
    </div>
  </section>
</template>

<script>
export default {};
</script>

<style lang="scss">
#portfolio-description {
  margin-top: 100px;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: flex-start;
  .portfolio-title {
  font-size: 35px;
    font-weight: 500;
     color: #D36B00;
  }
  .portfolio-desc {
    text-align: start !important;
    margin-top: 20px;

  }
}
</style>
