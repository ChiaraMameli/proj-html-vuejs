<template>
    <header>
        <HeaderMenu :NavLinks="NavLinks" />
        <HeaderJumbotron />
        <div class="d-flex justify-content-center">
            <div v-for="n in 3" :key="n" class="dot"></div>
            <div class="selected-dot"></div>
        </div>
    </header>
</template>

<script>
import HeaderMenu from "./HeaderMenu.vue";
import HeaderJumbotron from "./HeaderJumbotron.vue";
export default {
    name: "BaseHeader",
    components: { HeaderMenu, HeaderJumbotron },
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

    background: rgba(0, 0, 0, .3) url(../assets/img/header-slide-1.jpg);
    background-size: cover;
    background-position: center;
    background-blend-mode: darken;

    color: #FFF;

    .dot{
        height: 1rem;
        width: 1rem;
        border-radius: 50%;
        background-color: rgba(255, 255, 255, 0.5);
        margin-right: 0.5rem;

        cursor: pointer;

        &:hover{
            transform: scale(0.5);
            background-color: #FFF;
        }
    }
}

</style>