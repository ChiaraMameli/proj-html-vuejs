<template>
  <section class="container pt-5 pb-5 row">
    <div v-for="partner in Partners" :key="partner.id" class="col-3">
    <img :src="require(`../assets/img/${partner.imgUrl}.png`)" :alt="partner.label">
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
section{
    img{
        width: 50%;
    }
}

</style>