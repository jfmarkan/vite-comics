<template>
    <section>
        <div class="container">
            <div v-for="action in actions" class="action">
                <img :src="getImagePath(`../assets/img/${action.img}`)" alt="">
                <p>{{ action.text }}</p>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'AppBlueRow',
    data(){
        return{
            actions: [
                {
                    img: 'buy-comics-digital-comics.png',
                    text: 'DIGITAL COMICS'
                },
                {
                    img: 'buy-comics-merchandise.png',
                    text: 'DC MERCHANDISE'
                },
                {
                    img: 'buy-comics-subscriptions.png',
                    text: 'SUBSCRIPTION'
                },
                {
                    img: "buy-comics-shop-locator.png",
                    text: 'COMIC SHOP LOCATOR'
                },
                {
                    img: "buy-dc-power-visa.svg",
                    text: 'DC POWER VISA'
                }
            ]
        }
    },
    methods: {
        getImagePath: function (imgPath){
            return new URL(imgPath, import.meta.url).href;
        }
    }
}

</script>

<style lang="scss" scoped>
    @use '../styles/partials/mixins' as *;
    @use '../styles/partials/variables' as *;
    
    section{
        background-color: $blue-bg;


        .container{
            @include d-flex();
        
        .action{
            @include d-flex();

            img{
                width: 50px;
                margin: 2rem 1rem;
            }

            p{
                color: #FFF;
            }
        } 
    }
    }
</style>