<template>
  <section class="container align-items-center pt-5 pb-5">
    <div class="d-flex">
        <div class="text-center">
            <img src="../assets/img/joan-collins.jpg" alt="Joan Collins">
            <span class="testimonial-quote d-block pt-4">"Lorem ipsum dolor, sit amet consectetur adipisicing elit. Reprehenderit voluptas ad pariatur mollitia, voluptatum nemo ab libero debitis ut officiis cum fugit ipsam id? Recusandae dignissimos quaerat laboriosam modi esse!"</span>
            <span class="testimonial-name d-block pt-4">Joan Collins</span>
            <span class="testimonial-status d-block text-uppercase pt-2">student</span>
        </div>
    </div>

    <div id="dots" class="d-flex position-absolute start-50 translate-middle-x">
        <div v-for="n in 3" :key="n" class="dot"></div>
    </div>
  </section>
</template>

<script>
export default {
    name: 'SectionTestimonials'
}
</script>

<style scoped lang="scss">
@import '../assets/sass/utils';
    section{
        background-image: url(../assets/img/testimonials-background.png);
        background-size: cover;
        height: 600px;

        padding: 10rem;

        color: #fff;

        position: relative;

        img{
            border-radius: 50%;
            width: 15%;
            object-fit: contain;
            margin-top: 5rem;
        }

        span {
            font-family: sans-serif;
        }

        .testimonial-quote {
            font-weight: 100;
        }

        .testimonial-name{
            font-weight: 600;
            font-family: 'Noto Serif HK', serif;
        }

        .testimonial-quote,
        .testimonial-name {
            font-size: $text_size;

        }

        .testimonial-status {
            font-size: 0.8rem;
        }

        #dots{
            bottom: 6rem;
        }

        .dot{
        height: 1rem;
        width: 1rem;
        border-radius: 50%;
        background-color: rgba(255, 255, 255, 0.5);
        margin: 0 0.5rem;
        

        cursor: pointer;

        &:hover{
            transform: scale(0.5);
            background-color: #FFF;
        }
    }

    }
</style>