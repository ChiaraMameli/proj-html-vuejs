<template>
  <section class="container d-flex align-items-center pt-5 pb-5">
    <div class="text-center">
        <img src="../assets/img/joan-collins.jpg" alt="Joan Collins">
        <span class="d-block pt-2">Lorem ipsum dolor, sit amet consectetur adipisicing elit. Reprehenderit voluptas ad pariatur mollitia, voluptatum nemo ab libero debitis ut officiis cum fugit ipsam id? Recusandae dignissimos quaerat laboriosam modi esse!</span>
        <span class="d-block pt-2">Joan Collins</span>
        <span class="d-block text-uppercase pt-2">student</span>
    </div>
  </section>
</template>

<script>
export default {
    name: 'SectionTestimonials'
}
</script>

<style scoped lang="scss">
    section{
        height: 600px;
        background-image: url(../assets/img/testimonials-background.png);
        background-size: cover;

        padding: 10rem;

        color: #fff;

        img{
            border-radius: 50%;
            width: 10%;
        }
    }
</style>