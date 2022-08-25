<template>
  <div>
    <BaseHeader />
    <BaseMain />
    <BaseFooter />
  </div>
</template>

<script>
import BaseHeader from './components/BaseHeader.vue';
import BaseMain from './components/BaseMain.vue';
import BaseFooter from './components/BaseFooter.vue';
export default {
  name: 'App',
  components: {
    BaseHeader,
    BaseMain,
    BaseFooter
}
}
</script>

<style lang="scss">
@import 'bootstrap';
@import './assets/sass/style.scss';
@import url('https://fonts.googleapis.com/css2?family=Noto+Serif+HK:wght@200;300;400;600;700;800;900&display=swap');
*{
  font-family: 'Noto Serif HK', serif;
}
</style>
