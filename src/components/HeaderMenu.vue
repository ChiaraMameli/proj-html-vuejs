<template>
  <nav id="top-page" class="container d-flex justify-content-between">
    <div id="header-logo"><a href="#"><img src="../assets/img/logo-default.png" alt="iAcademy Logo"></a></div>
    <div>
        <ul  class="d-flex align-items-center h-100">
            <li v-for="item in NavLinks" :key="item.label"><a :href="item.link" class="text-white text-uppercase p-4">{{item.label}}</a></li>
        </ul>
    </div>
    <div>
        <ul id="header-menu-right" class="d-flex align-items-center h-100">
            <li><a href="#" class="text-white ps-4"><FontAwesomeIcon icon="fa-solid fa-magnifying-glass" /></a></li>
            <li class="position-relative" ><a href="#" class="text-white ps-4"><FontAwesomeIcon icon="fa-solid fa-bag-shopping" /><div class="item-bag position-absolute top-0">0</div></a></li>
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
@import '../assets/sass/colours';
nav{
    padding: 2rem;

    #header-logo{
        img{ 
            filter: invert(100%) sepia(54%) saturate(2%) hue-rotate(181deg) brightness(250%) contrast(101%);
            height: 2rem;
        }
    }

    .item-bag {
        height: 0.8rem;
        width: 0.8rem;
        background-color: $primary_colour;
        border-radius: 50%;

        left: 80%;

        font-size: 0.6rem;
        text-align: center;
        line-height: 0.8rem;
    }
}

</style>