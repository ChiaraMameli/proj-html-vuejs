<template>
  <section class="container pt-5 pb-5 text-center">
    <h3>Pricing Plans</h3>
    <span>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Voluptate velit hic sit aut possimus in eos, nihil ducimus</span>
    <div class="d-flex">
        <div class="my-table">
            <div class="my-table-head">Save up to 40% by paying weekly</div>
            <div class="my-table-data">Number of Courses</div>
            <div class="my-table-data">Time</div>
            <div class="my-table-data">Web Designing</div>
            <div class="my-table-data">Human Centered Design</div>
            <div class="my-table-data">Basic Marketing</div>
            <div class="my-table-data">Phyton for Everybody</div>
            <div class="my-table-data">Android Developer</div>
            <div class="my-table-data">Business English</div>
        </div>
        <div v-for="plan in PricingPlans" :key="plan.id" class="my-table">
            <div class="my-table-head">Save up to 40% by paying weekly</div>
            <div class="my-table-data">{{plan.numberOfCourses}}</div>
            <div class="my-table-data">{{plan.time}}</div>
            <div class="my-table-data">
                <span v-if="plan.webDesigning"><FontAwesomeIcon icon="fa-solid fa-check" /></span>
                <span v-else><FontAwesomeIcon icon="fa-solid fa-xmark" /></span>
            </div>
            <div class="my-table-data">
                <span v-if="plan.humanCenteredDesign"><FontAwesomeIcon icon="fa-solid fa-check" /></span>
                <span v-else><FontAwesomeIcon icon="fa-solid fa-xmark" /></span>
            </div>
            <div class="my-table-data">
                <span v-if="plan.basicMarketing"><FontAwesomeIcon icon="fa-solid fa-check" /></span>
                <span v-else><FontAwesomeIcon icon="fa-solid fa-xmark" /></span>
            </div>
            <div class="my-table-data">
                <span v-if="plan.phyton"><FontAwesomeIcon icon="fa-solid fa-check" /></span>
                <span v-else><FontAwesomeIcon icon="fa-solid fa-xmark" /></span>
            </div>
            <div class="my-table-data">
                <span v-if="plan.androidDeveloper"><FontAwesomeIcon icon="fa-solid fa-check" /></span>
                <span v-else><FontAwesomeIcon icon="fa-solid fa-xmark" /></span>
            </div>
            <div class="my-table-data">
                <span v-if="plan.businessEnglish"><FontAwesomeIcon icon="fa-solid fa-check" /></span>
                <span v-else><FontAwesomeIcon icon="fa-solid fa-xmark" /></span>
            </div>
            <div class="my-table-button">
                <button class="btn btn-primary">BUY</button>
            </div>

        </div>
    </div>

  </section>
</template>

<script>
export default {
    name: 'SectionPricingPlans',
    props: {PricingPlans:  Array}
}
</script>

<style scoped lang="scss">
@import '../assets/sass/colours';
    .my-table-head,
    .my-table-data,
    .my-table-button {
        width: calc(100 / 4);
        border: 1px solid $grey;
    }

    .my-table-head {
        height: 200px;
        padding: 3rem;
    }

    .my-table-data {
        height: 60px;
        padding: 1rem;

    }
    .my-table-button {
        height: 80px;
        padding: 1rem;

    }


</style>