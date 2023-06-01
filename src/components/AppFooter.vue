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
                    <a href="#">
                        <h5>DC COMICS</h5>
                    </a>
                    <ul>
                        <a href="#">
                            <li>Characters</li>
                        </a>
                        <a href="#">
                            <li>Comics</li>
                        </a>
                        <a href="#">
                            <li>Movies</li>
                        </a>
                        <a href="#">
                            <li>TV</li>
                        </a>
                        <a href="#">
                            <li>Games</li>
                        </a>
                        <a href="#">
                            <li>Videos</li>
                        </a>
                        <a href="#">
                            <li>News</li>
                        </a>
                    </ul>
                    <a href="#">
                        <h5>SHOP</h5>
                    </a>
                    <ul>
                        <a href="#">
                            <li>Shop DC</li>
                        </a>
                        <a href="#">
                            <li>Shop DC COllectibles</li>
                        </a>
                    </ul>
                </div>
                <div>
                    <a href="#">
                        <h5>DC COMICS</h5>
                    </a>
                    <ul>
                        <a href="#">
                            <li>Terms Of Use</li>
                        </a>
                        <a href="#">
                            <li>Privacy policy (New)</li>
                        </a>
                        <a href="#">
                            <li>Ad Choices</li>
                        </a>
                        <a href="#">
                            <li>Advertising</li>
                        </a>
                        <a href="#">
                            <li>Jobs</li>
                        </a>
                        <a href="#">
                            <li>Subscriptions</li>
                        </a>
                        <a href="#">
                            <li>Talent Workshops</li>
                        </a>
                        <a href="#">
                            <li>CPSC Certificates</li>
                        </a>
                        <a href="#">
                            <li>Ratings</li>
                        </a>
                        <a href="#">
                            <li>Shop Help</li>
                        </a>
                        <a href="#">
                            <li>Contact Us</li>
                        </a>
                    </ul>
                </div>
                <div>
                    <a href="#">
                        <h5>SITES</h5>
                    </a>
                    <ul>
                        <a href="#">
                            <li>DC</li>
                        </a>
                        <a href="#">
                            <li>MAD Magazine</li>
                        </a>
                        <a href="#">
                            <li>DC Kids</li>
                        </a>
                        <a href="#">
                            <li>DC Universe</li>
                        </a>
                        <a href="#">
                            <li>DC Power Visa</li>
                        </a>

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
            margin-bottom: 15px;

            a {
                color: $grey-font;

                &:hover {
                    color: $white-font;
                }

                li {
                    margin-bottom: 5px;
                }
            }
        }

        #dc-logo-bg {
            position: absolute;
            right: -20px;
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
}</style>

