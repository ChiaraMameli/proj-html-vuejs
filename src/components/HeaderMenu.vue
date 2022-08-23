<template>
  <nav class="container d-flex justify-content-between">
    <div><a href="#"><img src="../assets/img/logo-default.png" alt="iAcademy Logo"></a></div>
    <div>
        <ul class="d-flex">
            <li v-for="item in NavLinks" :key="item.label"><a :href="item.link" class="text-white text-uppercase">{{item.label}}</a></li>
        </ul>
    </div>
    <div>
        <ul class="d-flex">
            <li>i</li>
            <li>i</li>
            <li>i</li>
        </ul>
    </div>
  </nav>
</template>

<script>
export default {
    name: 'HeaderMenu',
    props: {
        NavLinks: Array
    }
}
</script>

<style scoped lang="scss">
@import '../assets/sass/style.scss';

</style>