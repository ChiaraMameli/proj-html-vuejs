<template>
  <section class="container pt-5 pb-5">
    <h3 class="pb-2">The Trusted Name for In-Home Tutoring</h3>
    <span class="d-block pb-2">Lorem ipsum dolor, sit amet consectetur adipisicing elit. Facilis soluta esse iusto minima numquam explicabo reprehenderit fugiat! Modi hic ipsum voluptas, debitis vero saepe! Inventore commodi nemo totam quisquam ratione.</span>
    <a href="#" class="text-uppercase">Learn More</a>
    <img src="../assets/img/students.jpg" alt="students" class="d-block">
  </section>
</template>

<script>
export default {
    name: 'TrudtedName'
}
</script>

<style scoped lang="scss">
@import '../assets/sass/colours';
section{
    h3{
        font-size: 2.9rem;
        color: $dark_grey;

        padding-right: 50rem;
    }

    span{
        color: $grey;
    }

    a{
        color: $primary_colour;
    }

    img{
        width: 100%;
    }
}
</style>