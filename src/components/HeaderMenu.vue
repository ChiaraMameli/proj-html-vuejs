<template>
  <nav class="container d-flex justify-content-between">
    <div id="header-logo"><a href="#"><img src="../assets/img/logo-default.png" alt="iAcademy Logo"></a></div>
    <div>
        <ul  class="d-flex align-items-center h-100">
            <li v-for="item in NavLinks" :key="item.label"><a :href="item.link" class="text-white text-uppercase p-2">{{item.label}}</a></li>
        </ul>
    </div>
    <div>
        <ul id="header-menu-right" class="d-flex align-items-center h-100">
            <li><a href="#" class="text-white ps-4"><FontAwesomeIcon icon="fa-solid fa-magnifying-glass" /></a></li>
            <li><a href="#" class="text-white ps-4"><FontAwesomeIcon icon="fa-solid fa-bag-shopping" /></a></li>
            <li><a href="#" class="text-white ps-4"><FontAwesomeIcon icon="fa-solid fa-bars" /></a></li>
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
nav{
    padding: 2rem;

    #header-logo{
        img{ 
            filter: invert(100%) sepia(54%) saturate(2%) hue-rotate(181deg) brightness(250%) contrast(101%);
            height: 2rem;
        }
    }
}

</style>