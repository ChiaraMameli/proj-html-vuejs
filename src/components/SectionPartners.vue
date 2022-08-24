<template>
  <section class="container pt-5 pb-5 row">
    <div v-for="partner in partners" :key="partner.id" class="col-3">
    <img :src="require(`../assets/img/${partner.imgUrl}.png`)" :alt="partner.label">
    </div>
  </section>
</template>

<script>
export default {
    name: 'SectionPartners',
    data(){
        return{
            partners:[
                {
                    id: 1,
                    label: 'Teach Hub',
                    imgUrl: 'teach-hub'
                },
                {
                    id: 2,
                    label: 'Study Central',
                    imgUrl: 'study-central'
                },
                {
                    id: 3,
                    label: 'Educator',
                    imgUrl: 'educator'
                },
                {
                    id: 4,
                    label: 'Scholar',
                    imgUrl: 'scholar'
                },


            ]
        }
    }
}
</script>

<style scoped lang="scss">
section{
    img{
        width: 50%;
    }
}

</style>