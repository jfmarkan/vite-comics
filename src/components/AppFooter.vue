<template>
    <footer>
        <div class="footer-top">
            <div class="container">
                <div class="navigation">
                    <div class="footer-col">
                        <h4>DC COMICS</h4>
                        <ul>
                            <li>Characters</li>
                            <li>Comics</li>
                            <li>Movies</li>
                            <li>TV</li>
                            <li>Games</li>
                            <li>Videos</li>
                            <li>News</li>
                        </ul>
                        <h4>SHOP</h4>
                        <ul>
                            <li>Shop DC</li>
                            <li>Shop DC Collectibles</li>
                        </ul>
                    </div>
                    <div class="footer-col">
                        <h4>DC</h4>
                        <ul>
                            <li>Terms Of Use</li>
                            <li>Privacy policy (New)</li>
                            <li>Ad Choices</li>
                            <li>Advertising</li>
                            <li>Jobs</li>
                            <li>Subscriptions</li>
                            <li>Talent Workshops</li>
                            <li>CPSC Certificates</li>
                            <li>Ratings</li>
                            <li>Shop Help</li>
                            <li>Contact Us</li>
                        </ul>
                    </div>
                    <div class="footer-col">
                        <h4>SITES</h4>
                        <ul>
                            <li>DC</li>
                            <li>MAD Magazine</li>
                            <li>DC Kids</li>
                            <li>DC Universe</li>
                            <li>DC Power Visa</li>
                        </ul>
                    </div>
                </div>
                <div class="logo">
                    
                </div>
            </div>
        </div>
        <div class="footer-bottom">
            <div class="container">
                <div class="action">
                    <button>SIGN-UP NOW!</button>
                </div>
                <div class="social-media">
                    <h4>FOLLOW US</h4>
                    <ul>
                        <li>
                            <img src="../assets/img/footer-facebook.png" alt="">
                        </li>
                        <li>
                            <img src="../assets/img/footer-twitter.png" alt="">
                        </li>
                        <li>
                            <img src="../assets/img/footer-youtube.png" alt="">
                        </li>
                        <li>
                            <img src="../assets/img/footer-pinterest.png" alt="">
                        </li>
                        <li>
                            <img src="../assets/img/footer-periscope.png" alt="">
                        </li>
                    </ul>
                </div>
            </div>
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
        height: 350px;
        .container{
            @include d-flex();
        
                .navigation{
                    @include d-flex(column, space-between, center, wrap);
                    height: 300px;

                    .footer-col{
                        margin: 0 1rem;
                    }

                    h4{
                        color: #FFF;
                        font-size: 1.25rem;
                        padding: .35rem 0
                    }

                    ul{
                        margin: .75rem 0;
                        color: #959595;
                        font-size: .8rem;
                        font-weight: 300;

                        li{
                            margin: .5rem 0
                        }
                    }
                }

                .logo{
                    background-image: url(../assets/img/dc-logo-bg.png);
                    background-size: cover;
                    background-position: center;
                    background-repeat: no-repeat;
                    height: 350px;
                    width: 39%;
                }
            }
        }

    .footer-bottom{
        background-color: $grey-bg;
        height: 85px;

        .container{
            @include d-flex();
            height: 100%;

            .action{

                button{
                    border: $blue-bg 2px solid;
                    color:#FFF;
                    padding: .5rem;
                    font-size: 1rem;
                    font-weight: 600;
                    background-color: $grey-bg;
                }
            }

            .social-media{
                @include d-flex();

                h4{
                    font-size: 1.25rem;
                    color: $blue-bg;
                }

                ul{
                    @include d-flex();

                    li{
                        margin-left:1.25rem;
                    }
                }
            }
        }

        

    }
</style>