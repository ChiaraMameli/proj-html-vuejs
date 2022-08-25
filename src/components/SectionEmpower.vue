<template>
  <section class="container pt-5 pb-5">
    <div class="row">
        <div id="image-section" class="col-6">
            <img src="../assets/img/world-hands.jpg" alt="Hands holding the world">
        </div>
        <div class="col-6 pe-5">
            <h4 class="pb-4">Empowering Children to Reach Their Potential</h4>
            <span class="d-block pb-4">Lorem ipsum dolor, sit amet consectetur adipisicing elit. Facilis soluta esse iusto minima numquam explicabo reprehenderit fugiat! Modi hic ipsum voluptas, debitis vero saepe! Inventore commodi nemo totam quisquam ratione.</span>
            <div id="empowering-data" class="row justify-content-between">
                <div class="col-6">
                   <span class="d-block empowering-data-num">168</span> 
                   <span>Users Stories</span>
                </div>
                <div class="col-6">
                    <span class="d-block empowering-data-num">347</span> 
                    <span>Events</span>
                </div>
            </div>
        </div>
    </div>
  </section>
</template>

<script>
export default {
    name: 'SectionEmpower'
}
</script>

<style scoped lang="scss">
@import '../assets/sass/colours';
@import '../assets/sass/utils';

    section{

        #image-section{
            img{
                width: 20rem;
                margin-left: 10rem;
            }
        }
       
        h4{
            font-size: $h4_size;
            color: $dark_grey;
            font-weight: 700;
        }

        span{
        color: $grey;
        font-size: $span_size;
        font-family: sans-serif;
        font-weight: 100;

        }

        #empowering-data{

            span{
            color: $primary_colour;
            font-family: 'Noto Serif HK', serif;
            font-weight: 600;
            }

            .empowering-data-num{
            font-size: 3rem;
            }
        }
        
    }
</style>