<template>
        <article>
            <img :src="comicElement.thumb" alt="">
            <p>{{ comicElement.series.toUpperCase() }}</p>
        </article>
</template>

<script>
export default {
    name: 'SingleProduct',
    props: {
        comicElement : Object
    },
}
</script>

<style lang="scss" scoped>
    article{
        width: calc((100vw / 9) - 20px);
        margin-top: 2rem;

        img{
            width: 100%;
            height: calc(100vw / 9);


            margin-bottom: 1rem;
        }

        p{
            color: #FFF;
            font-size: .9rem;
        }
    }
</style>