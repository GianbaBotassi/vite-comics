<script>
import AppMerchandise from './AppMerchandise.vue'


export default {
    components: {
        AppMerchandise,
    },
    name: "AppFooter"
}
</script>

<template>
    <footer>
        <AppMerchandise />
        <div id="content-bg">
            <div id="content-info" class="container">
                <div>
                    <h5>DC COMICS</h5>
                    <ul>
                        <li>Characters</li>
                        <li>Comics</li>
                        <li>Movies</li>
                        <li>TV</li>
                        <li>Games</li>
                        <li>Videos</li>
                        <li>News</li>
                    </ul>
                    <h5>SHOP</h5>
                    <ul>
                        <li>Shop DC</li>
                        <li>Shop DC COllectibles</li>
                    </ul>
                </div>
                <div>
                    <h5>DC COMICS</h5>
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
                <div>
                    <h5>SITES</h5>
                    <ul>
                        <li>DC</li>
                        <li>MAD Magazine</li>
                        <li>DC Kids</li>
                        <li>DC Universe</li>
                        <li>DC Power Visa</li>

                    </ul>
                </div>
                <div id="dc-logo-bg">
                    <img src="../assets/img/dc-logo-bg.png" alt="logo-bg">
                </div>
            </div>



        </div>
        <div id="foot-bar">
            <div id="foot-social" class="container">
                <a id="foot-left" href="#">
                    SIGN-UP NOW!
                </a>
                <div id="foot-right">
                    <div id="follow">FOLLOW US</div>
                    <div id="social">
                        <div>
                            <a href="#">
                                <img src="../assets/img/footer-facebook.png" alt="facebook">
                            </a>
                            <a href="#">
                                <img src="../assets/img/footer-twitter.png" alt="twitter">
                            </a>
                            <a href="#">
                                <img src="../assets/img/footer-youtube.png" alt="youtube">
                            </a>
                            <a href="#">
                                <img src="../assets/img/footer-pinterest.png" alt="pinterest">
                            </a>
                            <a href="#">
                                <img src="../assets/img/footer-periscope.png" alt="periscope">
                            </a>
                        </div>
                    </div>
                </div>
            </div>
        </div>

    </footer>
</template>

<style lang="scss" scoped>
@use 'styles/partials/mixins' as *;
@use 'styles/partials/variables' as *;

footer {
    height: calc(100% - 200px);

    #content-bg {
        background-image: url(../assets/img/footer-bg.jpg);
    }

    #content-info {
        display: flex;
        justify-content: flex-start;
        gap: 25px;
        color: $white-font;
        padding: 20px 0;
        position: relative;
        overflow: hidden;

        h5 {
            margin-bottom: 15px;
        }

        ul {
            font-size: 0.6rem;
            color: $grey-font;
            margin-bottom: 15px;

            li {
                margin-bottom: 5px;
            }
        }

        #dc-logo-bg {
            position: absolute;
            right: 40px;
            bottom: -50px;

            img {
                height: 400px;
            }
        }

    }

    #foot-bar {
        font-size: 0.8rem;
        background-color: $grey;
        height: 100px;
        @include flex-content(between);

        #foot-social {
            @include flex-content(between);

            #foot-left {
                border: 2px solid $blue;
                color: $white-font;
                padding: 10px;

                &:hover {
                    background-color: lighten($color: blue, $amount: 20%)
                }
            }

            #foot-right {
                @include flex-content(between);
                color: $blue;
                gap: 10px;

                img {
                    margin-right: 10px;
                    height: 25px;
                }
            }
        }
    }
}
</style>

