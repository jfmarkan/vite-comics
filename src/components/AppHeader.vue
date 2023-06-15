<template>
    <header>
        <div class="container">
            <div>
                <img src="" alt="">
            </div>
            <div>
                <nav>
                    <ul>
                        <li>
                            10
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
    
</style>