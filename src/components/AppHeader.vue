<template>
    <header>
        <div class="container">
            <div>
                <img src="../assets/img/dc-logo.png" alt="DC Logo">
            </div>
            <div>
                <nav>
                    <ul>
                        <li v-for="link in topLinks" :class="active ==='true' ? 'active' : ''">
                            {{link.text}}
                        </li>
                    </ul>
                </nav>
            </div>
        </div>
    </header>
</template>

<script>
export default {
    name: 'AppHeader',
    data(){
        return{
            topLinks: [
                {
                    text: 'CHARACTERS',
                    active: false,
                },
                {
                    text: 'COMICS',
                    active: true,
                },
                {
                    text: 'MOVIES',
                    active: false,
                },
                {
                    text: 'TV',
                    active: false,
                },
                {
                    text: 'GAMES',
                    active: false,
                },
                {
                    text: 'COLLECTIBLES',
                    active: false,
                },
                {
                    text: 'VIDEOS',
                    active: false,
                },
                {
                    text: 'FANS',
                    active: false,
                },
                {
                    text: 'NEWS',
                    active: false,
                },
                {
                    text: 'SHOP',
                    active: false,
                },
            ]
        }
    }
}
</script>

<style lang="scss">
    @use '../styles/partials/mixins' as *;
    @use '../styles/partials/variables' as *;

    header{
        height: 90px;
    }

    div.container{
        @include d-flex();

        ul{
            @include d-flex();

            li{
                margin-left: .5rem;
            }
        }

        img{
            width: 70%
        }
    }
</style>