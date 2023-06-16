<template>
    <header>
        <div class="container">
            <div>
                <img src="../assets/img/dc-logo.png" alt="DC Logo">
            </div>
            <div>
                <nav>
                    <ul>
                        <li v-for="link in topLinks" :class="link.active ? 'active' : ''">
                            {{link.text}}
                            <div :class="link.active ? 'highlighted' : ''"></div>
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
            ],
        }
    },
}
</script>

<style lang="scss" scoped>
    @use '../styles/partials/mixins' as *;
    @use '../styles/partials/variables' as *;

    div.container{
        @include d-flex();
        padding: calc($section-padding / 2) 0;

        ul{
            @include d-flex();

            li{
                margin-left: 1rem;
                font-weight: 500;
                font-size: .8rem;
                position: relative;
            }
        }

        img{
            width: 70%
        }
    }
    .active{
        color: $blue-highlight;
    }

    .highlighted{
        width: 40px;
        height: 5px;
        background-color: $blue-bg;
        position: absolute;
        top: 56px;
        transform: translateX(-50%);
        left: 50%;
    }
</style>