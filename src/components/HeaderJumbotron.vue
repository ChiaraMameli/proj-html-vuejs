<template>
    <div id="jumbotron" class="d-flex justify-content-center align-items-center text-center">
        <div>
            <h2>Contemporary Ideas</h2>
            <span class="d-block">Lorem ipsum dolor sit amet consectetur adipisicing elit. Provident et accusamus vitae voluptatem vel deleniti 
                hic delectus, neque, ipsam nihil enim repudiandae tempore corrupti harum ut voluptate molestias deserunt placeat!
            </span>
            <button type="button" class="_bttn">REGISTER NOW</button>
        </div>
    </div>
</template>

<script>
export default {
    name: 'HeaderJumbotron'
}
</script>

<style scoped lang="scss">
@import '../assets/sass/colours';

#jumbotron {
    padding: 10rem;

    h2{
        font-size: 4.5rem;
        font-weight: 700;
    }

    span {
        padding: 2rem 5rem;
    }

    ._bttn {
    font-size: 0.8rem;
    font-weight: 500;
    font-family: sans-serif;
    color: #FFF;

    padding: 0.7rem 2rem;
    background-color: $primary_colour;
    border: 2px solid $primary_colour;

    &:hover {
        background-color: transparent;
        color: #FFF;
        border: 2px solid #FFF;

    }
    }

}
</style>