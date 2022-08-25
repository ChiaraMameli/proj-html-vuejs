<template>
    <a href="#top-page"><FontAwesomeIcon icon="fa-solid fa-angle-up" /><br />TOP</a>
</template>

<script>
export default {
    name: 'TopButton'
}
</script>

<style scoped lang="scss">
@import '../assets/sass/colours';
    a{
        height: 3rem;
        width: 3rem;
        background-color: $primary_colour;
        border: none;
        padding: 0.2rem;

        color: #FFF;
        font-size: 0.8rem;
        text-align: center;

        position: fixed;
        right: 52px;
        bottom: 20px;

        &:hover {
            color: #FFF;
        }
    }
</style>