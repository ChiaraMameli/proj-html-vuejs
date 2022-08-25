<template>
  <footer>
    <FooterTop />
    <FooterBottom />
  </footer>
</template>

<script>
import FooterTop from './FooterTop.vue';
import FooterBottom from './FooterBottom.vue';
export default {
    name: "BaseFooter",
    components: { FooterTop, FooterBottom }
}
</script>

<style scoped lang="scss">
@import '../assets/sass/colours';

footer{
    padding-top: 5rem;
    background-color: $footer_colour ;
}
</style>