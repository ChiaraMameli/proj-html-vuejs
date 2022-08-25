<template>
  <section class="container pt-5 pb-5">
    <div class="row">
      <div v-for="partner in Partners" :key="partner.id" class="col-3 text-centeral ">
        <a :href="partner.link"><img :src="require(`../assets/img/${partner.imgUrl}.png`)" :alt="partner.label"></a>
      </div>
    </div>
  </section>
</template>

<script>
export default {
    name: 'SectionPartners',
    props:{Partners: Array}
}
</script>

<style scoped lang="scss">
@import '../assets/sass/colours';

section{
  border-top: 1px solid $border_colour;

    img{
        width: 100%;
        cursor: pointer;
    }
}

</style>