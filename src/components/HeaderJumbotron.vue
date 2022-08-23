<template>
    <div id="jumbotron" class="d-flex justify-content-center align-items-center text-center">
        <div>
            <h2>Contemporary Ideas</h2>
            <span class="d-block">Lorem ipsum dolor sit amet consectetur adipisicing elit. Provident et accusamus vitae voluptatem vel deleniti 
                hic delectus, neque, ipsam nihil enim repudiandae tempore corrupti harum ut voluptate molestias deserunt placeat!
            </span>
            <button type="button" class="btn btn-primary">clicca</button>
        </div>
    </div>
</template>

<script>
export default {
    name: 'HeaderJumbotron'
}
</script>

<style scoped lang="scss">
#jumbotron {
    padding: 10rem;

    h2{
        font-size: 4.5rem;
    }

    span {
        padding: 2rem 5rem;
    }
}
</style>