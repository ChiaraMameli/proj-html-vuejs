<template>
  <section class="container d-flex align-items-center pt-5 pb-5">
    <div class="text-center">
        <img src="../assets/img/joan-collins.jpg" alt="Joan Collins">
        <span class="testimonial-quote d-block pt-4">"Lorem ipsum dolor, sit amet consectetur adipisicing elit. Reprehenderit voluptas ad pariatur mollitia, voluptatum nemo ab libero debitis ut officiis cum fugit ipsam id? Recusandae dignissimos quaerat laboriosam modi esse!"</span>
        <span class="testimonial-name d-block pt-4">Joan Collins</span>
        <span class="testimonial-status d-block text-uppercase pt-2">student</span>
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

        img{
            border-radius: 50%;
            width: 10%;
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
    }
</style>