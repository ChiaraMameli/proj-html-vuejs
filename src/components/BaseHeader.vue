<template>
    <header>
        <HeaderMenu />
    </header>
</template>

<script>
import HeaderMenu from "./HeaderMenu.vue";
export default {
    name: "BaseHeader",
    components: { HeaderMenu }
}
</script>

<style scoped lang="scss">
@import '../assets/sass/colours';

header{
    height: 700px;

    background-image: url(../assets/img/header-slide-1.jpg);
    background-size: cover;
    background-position: center;
}

</style>