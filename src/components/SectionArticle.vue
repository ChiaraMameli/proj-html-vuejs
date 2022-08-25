<template>
  <section class="container pt-5 pb-5">
    <div class="row">
        <div class="col-3">
            <div v-for="link in ArticleLinks" :key="link.id" class="slot">
                <span>{{link.label}}</span>
            </div>
        </div>
        <article class="col-9">
            <h4 class="pb-4">Learning Possibilities</h4>
            <span class="d-block pb-4">Lorem ipsum dolor, sit amet consectetur adipisicing elit. Facilis soluta esse iusto minima numquam explicabo reprehenderit fugiat! Modi hic ipsum voluptas, debitis vero saepe! Inventore commodi nemo totam quisquam ratione.</span>
            <ul>
                <li class="pb-4"><FontAwesomeIcon class="check-icon pe-2" icon="fa-solid fa-check" /> We enrich lives through learning</li>
                <li class="pb-4"><FontAwesomeIcon class="check-icon pe-2" icon="fa-solid fa-check" /> Maximizing potential through individual attention</li>
                <li class="pb-4"><FontAwesomeIcon class="check-icon pe-2" icon="fa-solid fa-check" /> The trusted Name for specialized training</li>
                <li class="pb-4"><FontAwesomeIcon class="check-icon pe-2" icon="fa-solid fa-check" /> People teach. People learn. This is how they connect.</li>
            </ul>
            <img id="stationary-image" src="../assets/img/stationery.png" alt="">
        </article>
    </div>
  </section>
</template>

<script>
export default {
    name: 'SectionArticle',
    props:{
        ArticleLinks: Array,
    }
}
</script>

<style scoped lang="scss">
@import '../assets/sass/colours';
@import '../assets/sass/utils';
    section{
        margin-top: 5rem;
        margin-bottom: 5rem;
        
        .slot{
            width: 18rem;
            padding: 1.5rem;
            border: 1px solid $border_colour;
            font-weight: 600;
            color: $text_colour;

            &:hover{
                cursor: pointer;
                color: $primary_colour;
                border-left: 5px solid $primary_colour;
                background-color: $fill_colour;
            }
        }

        article{

            position: relative;

            h4{
                font-size: $title_size;
                color: $title_colour;
                font-weight: 700;
            }

            span, li{
            color: $text_colour;
            }

            .check-icon{
                color: $primary_colour;
            }

            #stationary-image {
                width: 8rem;
                position: absolute;
                right: 300px;
                bottom: 100px;
            }
            
        }
    }

</style>