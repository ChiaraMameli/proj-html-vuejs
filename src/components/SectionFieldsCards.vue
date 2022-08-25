<template>
  <section class="container pt-5 pb-5">
    <div class="row justify-content-between pt-5 pb-5">
        <div v-for="field in Fields" :key="field.id" class="col-2 _card p-4 text-center">
            <img :src="require(`../assets/img/${field.imgUrl}.png`)" :alt="field.label" class="p-4">
            <h5 class="text-capitalize p-4">{{field.label}}</h5>
        </div>
    </div>
  </section>
</template>

<script>
export default {
    name: 'SectionFieldsCards',
    props:{
        Fields: Array
    },
}
</script>

<style scoped lang="scss">
@import '../assets/sass/colours';
._card{
    width: calc((100% / 6) - 1.5rem);
    background-color: $primary_background_colour;
    border-radius: 0.5rem;

    cursor: pointer;

    h5{
        font-weight: 600;
    }
}
</style>