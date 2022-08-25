<template>
  <section class="container pt-5 pb-5 text-center">
    <h3>Pricing Plans</h3>
    <span>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Voluptate velit hic sit aut possimus in eos, nihil ducimus</span>
    <div class="d-flex">
        <div class="my-table" id="table-indicator">
            <div class="my-table-head d-flex">Save up to 40% by paying weekly</div>
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
            <div class="my-table-head selectable">
                <img :src="require(`../assets/img/${plan.imgUrl}.png`)" :alt="plan.label">
                <h4 class="plan-label">{{plan.label}}</h4>
                <span class="plan-price">{{plan.price}}</span>
            </div>
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
                <button type="button" class="_bttn">GET IT NOW</button>
            </div>
        </div>
        <div class="label red-label"><img src="../assets/img/svg-0.svg" alt=""></div>
        <div class="label"><img src="../assets/img/svg-2.svg" alt=""></div>
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
@import '../assets/sass/utils';

    section{
        margin-bottom: 5rem;
        background: rgba(247, 249, 248, 0.2) url(../assets/img/page-background-img.png);
        background-size: cover;

        position: relative;

        h3{
            margin-top: 5rem;
            font-size: 3rem;
            color: $title_colour;
            font-weight: 700;
        }

        span{
            font-size: $text_size;
            color: #606264;
            font-family: sans-serif;
            font-weight: 100;
        }
    }

    .my-table{
        margin-top: 5rem;
        background-color: #FFF;

        & .selectable{
            background-color: $lighter_blue;

            &:hover {
                border-top: 5px solid $primary_colour;
            }
        }
    }

    #table-indicator 
    .my-table-data{
        font-weight: 600;
        color: $text_colour;
        text-align: left;
    }

    .my-table-head,
    .my-table-data,
    .my-table-button {
        border: 1px solid $border_colour;
        width: 20rem;
    }

    .my-table-head {
        height: 300px;
        padding: 3rem;
    }

    .my-table-head,
    .plan-label,
    .plan-price {
        font-size: 1.5rem;
        color: $title_colour;
        font-weight: 700;

    }

    .plan-label {
        margin-top: 1rem;
    }

    .my-table-data {
        height: 60px;
        padding: 1rem;
        color: $text_colour;

    }
    .my-table-button {
        height: 80px;
        padding: 1rem;

    }

    .fa-check{
        color: $primary_colour;
    }

    .fa-xmark {
        color: $text_colour;
    }

    ._bttn {
        font-size: 0.8rem;
        font-weight: 500;
        font-family: sans-serif;
        color: $text_colour;

        padding: 0.7rem 2rem;
        background-color: #FFF;
        border: 2px solid $border_colour;

        &:hover {
            background-color: $primary_colour;
            color: #FFF;
        }
    }

    .label{
        height: 3rem;
        width: 3rem;
        background-color: #FFF;
        border: none;
        padding: 0.5rem;

        position: absolute;
        left: 98%;
        bottom: 745px;

        box-shadow: 1px 1px 3px #606264;

    }

    .red-label{
        background-color: #EE2852;
        bottom: 800px;

    }

</style>