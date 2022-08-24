<template>
  <section class="container pt-5 pb-5">
    <h3>Popular Online Courses</h3>
    <span class="d-block p-5">Lorem ipsum, dolor sit amet consectetur adipisicing elit. Officia laudantium sed ad, beatae ipsum sint repudiandae quae amet repellat voluptatum at atque neque tempore cum dolorem quibusdam fugit. Voluptas, sapiente.</span>
    <div class="row justify-content-between">
        <div v-for="plan in PopularPlans" :key="plan.id" class="col-3 _card">
            <img :src="require(`../assets/img/${plan.imgUrl}.jpg`)" alt="Android Developer">
            <div class="p-4">
                <h5>{{plan.title}}</h5>
                <span class="d-block pt-2 pb-2">{{plan.teacheer}}</span>
                <span class="d-block">{{plan.description}}</span>
                <FontAwesomeIcon icon="fa-solid fa-user" /> <span>{{plan.numberOfPeople}}</span>
                <FontAwesomeIcon icon="fa-solid fa-tag" /> <span>{{plan.field}}</span>

            </div>
        </div>
    </div>
  </section>
</template>

<script>
export default {
    name: 'SectionPopularPlans',
    props:{
        PopularPlans: Array,
    },
}
</script>

<style scoped lang="scss">
@import '../assets/sass/colours';
    section{
        border-top: 1px solid $grey;
        border-bottom: 1px solid $grey;

        text-align: center;

        ._card{
            border: 1px solid $grey;

            img{
                width: 100%;
            }
        }
    }
</style>