<template>
    <footer>
        <div class="footer-top">
            <div class="container">
                <div class="navigation">
                    <nav>
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
                        <h4>SITES</h4>
                        <ul>
                            <li>DC</li>
                            <li>MAD Magazine</li>
                            <li>DC Kids</li>
                            <li>DC Universe</li>
                            <li>DC Power Visa</li>
                        </ul>
                    </nav>
                </div>
                <div class="logo">
                    
                </div>
            </div>
        </div>
        <div class="footer-bottom">
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
        
                .navigation{
                    padding: $section-padding;
                }
                .logo{
                    background-image: url(../assets/img/dc-logo-bg.png);
                    background-position: center;
                    background-repeat: no-repeat;
                    height: 300px;
                    width: 60%;
                }
            }
        }

    .footer-bottom{
        background-color: $grey-bg;
        height: 85px;
    }
</style>