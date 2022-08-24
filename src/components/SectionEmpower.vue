<template>
  <section class="container pt-5 pb-5">
    <div class="row">
        <div class="col-6">
            <img src="../assets/img/world-hands.jpg" alt="Hands holding the world">
        </div>
        <div class="col-6">
            <h3 class="pb-2">Empowering Children to Reach Their Potential</h3>
            <span class="d-block pb-2">Lorem ipsum dolor, sit amet consectetur adipisicing elit. Facilis soluta esse iusto minima numquam explicabo reprehenderit fugiat! Modi hic ipsum voluptas, debitis vero saepe! Inventore commodi nemo totam quisquam ratione.</span>
            <div id="empowering-data" class="d-flex justify-content-between">
                <div>
                   <span class="d-block empowering-data-num">168</span> 
                   <span>Users Stories</span>
                </div>
                <div>
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

    section{
        img{
            width: 70%;
        }
       
        h3{
            font-size: 2.9rem;
            color: $dark_grey;
        }

        span{
        color: $grey;
        }

        #empowering-data{

            span{
            color: $primary_colour;
            }
            .empowering-data-num{
                font-size: 3rem;
            }
        }
        
    }
</style>