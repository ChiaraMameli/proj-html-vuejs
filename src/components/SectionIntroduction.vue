<template>
  <section class="container pt-5 pb-5">
    <h4 class="pb-2">The Trusted Name for In-Home Tutoring</h4>
    <span class="d-block pb-4">Lorem ipsum dolor, sit amet consectetur adipisicing elit. Facilis soluta esse iusto minima numquam explicabo reprehenderit fugiat! Modi hic ipsum voluptas, debitis vero saepe! Inventore commodi nemo totam quisquam ratione.</span>
    <a href="#" class="text-uppercase">Learn More</a>
    <img src="../assets/img/students.jpg" alt="students" class="d-block">
  </section>
</template>

<script>
export default {
    name: 'SectionIntroduction'
}
</script>

<style scoped lang="scss">
@import '../assets/sass/colours';

section{
    h4{
        font-size: 2.5rem;
        font-weight: 700;
        color: $dark_grey;

        width: 35%;
    }

    span, a {
        font-family: sans-serif;
    }

    span{
        color: $grey;
        font-size: 1.2rem;
        font-weight: 100;
    }

    a{
        color: $primary_colour;
        font-size: 0.8rem;
    }

    img{
        width: 90%;
        margin: 0 auto;
    }
}
</style>