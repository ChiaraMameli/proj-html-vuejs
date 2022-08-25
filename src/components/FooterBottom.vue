<template>
  <section class="container pt-5 pb-5">
    <div class="row">
      <div class="col-6">
        Copyrights 2017 <FontAwesomeIcon icon="fa-solid fa-copyright" />Mikado Themes
      </div>
      <div class="col-6 text-end">
        <span class="d-inline-block pe-4">CALL +44 300 303 0266</span>
        <span class="d-inline-block pe-4">FOLLOW US</span>
        <span class="d-inline-block pe-4"><FontAwesomeIcon icon="fa-brands fa-twitter" /></span>
        <span class="d-inline-block pe-4"><FontAwesomeIcon icon="fa-brands fa-instagram" /></span>
        <span class="d-inline-block"><FontAwesomeIcon icon="fa-brands fa-facebook" /></span>

      </div>
    </div>
  </section>
</template>

<script>
export default {
    name: 'FooterBottom'
}
</script>

<style scoped lang="scss">
@import '../assets/sass/colours';
*{
  color: $text_colour;
  font-weight: 100;
  font-family: sans-serif;
  font-size: 0.9rem;
}
</style>