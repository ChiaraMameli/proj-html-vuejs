<template>
  <div class="container pt-5">
    <div class="d-flex justify-content-between">
        <div v-for="field in LearningFields" :key="field.id" class="_card p-4">
            <img :src="require(`../assets/img/${field.imgUrl}.png`)" :alt="field.label" class="p-4">
            <h5 class="p-4">{{field.label}}</h5>
        </div>
    </div>
  </div>
</template>

<script>
export default {
    name: 'LearningFieldsCards',
    props:{
        LearningFields: Array
    }
}
</script>

<style scoped lang="scss">
@import '../assets/sass/colours';
._card{
    background-color: $light_blue;
    border-radius: 0.5rem;
}
</style>