<template>
    <header>
        <HeaderMenu :NavLinks="NavLinks" />
    </header>
</template>

<script>
import HeaderMenu from "./HeaderMenu.vue";
export default {
    name: "BaseHeader",
    components: { HeaderMenu },
    data(){
    return{
        NavLinks: [
            {
                label: 'home',
                link: '#'
            },
            {
                label: 'courses',
                link: '#'
            },
            {
                label: 'instructions',
                link: '#'
            },
            {
                label: 'events',
                link: '#'
            },
            {
                label: 'pages',
                link: '#'
            },
            {
                label: 'elements',
                link: '#'
            }
            ]
        }
    }

}
</script>

<style scoped lang="scss">
@import '../assets/sass/colours';

header{
    height: 700px;

    background-image: url(../assets/img/header-slide-1.jpg);
    background-size: cover;
    background-position: center;

    color: #FFF;
}

</style>