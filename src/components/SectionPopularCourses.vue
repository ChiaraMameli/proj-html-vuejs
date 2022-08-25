<template>
  <section class="container pt-5 pb-5">
    <h3>Popular Online Courses</h3>
    <span class="d-block pt-2 pb-5">Lorem ipsum, dolor sit amet consectetur adipisicing elit. Officia laudantium sed ad, beatae ipsum sint repudiandae quae amet repellat voluptatum at atque neque tempore cum dolorem quibusdam fugit. Voluptas, sapiente.</span>
    <div class="row justify-content-between pt-5">
        <div v-for="course in PopularCourses" :key="course.id" class="col-3 _card">
            <img :src="require(`../assets/img/${course.imgUrl}.jpg`)" alt="Android Developer">
            <div class="p-4">
                <h5 class="m-0">{{course.title}}</h5>
                <span class="course-teacher d-block pt-2 pb-2">{{course.teacher}}</span>
                <span class="course-description d-block pb-2">{{course.description}}</span>
                <FontAwesomeIcon class="course-icon" icon="fa-solid fa-user" /> <span class="course-generic-data">{{course.numberOfPeople}}</span>
                <FontAwesomeIcon class="course-icon" icon="fa-solid fa-tag" /> <span class="course-generic-data text-uppercase">{{course.field}}</span>
            </div>
        </div>
    </div>
  </section>
</template>

<script>
export default {
    name: 'SectionPopularCourses',
    props:{
        PopularCourses: Array,
    },
}
</script>

<style scoped lang="scss">
@import '../assets/sass/colours';
@import '../assets/sass/utils';

    section{
        border-top: 1px solid $border_colour;
        border-bottom: 1px solid $border_colour;

        background: rgba(247, 249, 248, 0.2) url(../assets/img/page-background-img.png);
        background-size: cover;


        text-align: center;

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

        ._card{
            border: 1px solid $border_colour;
            background-color: #FFF;
            margin-bottom: 5rem;
            padding: 0;

            text-align: left;

            img{
                width: 100%;
            }

            h5{
                font-size: 1rem;
                color: $title_colour;
                font-weight: 700;
            }

            .course-teacher {
                font-size: 0.9rem;
                color: #B9B9B9;
                font-weight: 200;
            }

            .course-description {
                font-size: 1rem;
                font-weight: 100;
                color: $text_colour;
            }

            .course-icon{
                padding-right: 0.2rem;
            }

            .course-generic-data {
                padding-right: 0.6rem;
            }

            .course-icon,
            .course-generic-data {
                color: #B9B9B9;
                font-size: 0.8rem;
                font-weight: 500;
            }
        }
    }
</style>