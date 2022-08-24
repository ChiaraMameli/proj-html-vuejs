<template>
  <section class="container pt-5 pb-5">
    <div class="row">
        <div class="col-4">
            <div v-for="link in ArticleLinks" :key="link.id" class="slot">
                <span>{{link.label}}</span>
            </div>
        </div>
        <article class="col-8">
            <h3 class="pb-2">Learning Possibilities</h3>
            <span class="d-block pb-2">Lorem ipsum dolor, sit amet consectetur adipisicing elit. Facilis soluta esse iusto minima numquam explicabo reprehenderit fugiat! Modi hic ipsum voluptas, debitis vero saepe! Inventore commodi nemo totam quisquam ratione.</span>
            <ul>
                <li><FontAwesomeIcon class="check-icon" icon="fa-solid fa-check" /> We enrich lives through learning</li>
                <li><FontAwesomeIcon class="check-icon" icon="fa-solid fa-check" /> Maximizing potential through individual attention</li>
                <li><FontAwesomeIcon class="check-icon" icon="fa-solid fa-check" /> The trusted Name for specialized training</li>
                <li><FontAwesomeIcon class="check-icon" icon="fa-solid fa-check" /> People teach. People learn. This is how they connect.</li>

            </ul>
        </article>
    </div>
  </section>
</template>

<script>
export default {
    name: 'SectionArticle',
    data(){
        return{
            ArticleLinks:[
                {
                    label: 'What We Do',
                    id: 1,
                },
                                {
                    label: 'Degree Programme',
                    id: 2,
                },
                {
                    label: 'Career Achievements'
                },
                {
                    label: 'Personal Management',
                    id: 4,
                },
                {
                    label: 'Steps To Success',
                    id: 5,
                },
                {
                    label: 'Knowledge Transfer',
                    id: 6,
                },
            ]
        }
    }
}
</script>

<style scoped lang="scss">
@import '../assets/sass/colours';
    .slot{
        width: 20rem;
        padding: 1.5rem;
        border: 1px solid $grey;

        &:hover{
            cursor: pointer;
            color: $primary_colour;
            border-left: 5px solid $primary_colour;
        }
    }

    article{

        h3{
            font-size: 2.9rem;
            color: $dark_grey;
        }

        span, li{
        color: $grey;
        }

        .check-icon{
            color: $primary_colour;
        }
        
    }


</style>