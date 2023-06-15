<template>
    <footer>
        <div class="footer-top">
            <div class="container">
                <div class="navigation">
                    <nav>

                    </nav>
                </div>
                <div class="logo">
                    
                </div>
            </div>
        </div>
        <div class="footer-bottom">

        </div>
    </footer>
</template>

<script>
export default {
    name: 'AppFooter',
}
</script>

<style lang="scss" scoped>
    @use '../styles/partials/mixins' as *;
    @use '../styles/partials/variables' as *;

    .footer-top{
        background-image: url(../assets/img/footer-bg.jpg);
        height: 300px;

        .container{
            @include d-flex();

            .logo{
                background-image: url(../assets/img/dc-logo-bg.png);
                background-position: center;
                background-repeat: no-repeat;
                height: 300px;
                width: 45%;
            }
        }
    }

    .footer-bottom{
        background-color: $grey-bg;
        height: 85px;
    }
</style>