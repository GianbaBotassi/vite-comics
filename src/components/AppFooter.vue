<script>
import AppMerchandise from './components/AppMerchandise.vue'


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
        <div id="content-info" class="container">
            <div>
                <h3>DC COMICS</h3>
                <ul>
                    <li>Characters</li>
                    <li>Comics</li>
                    <li>Movies</li>
                    <li>TV</li>
                    <li>Games</li>
                    <li>Videos</li>
                    <li>News</li>
                </ul>
                <h3>SHOP</h3>
                <ul>
                    <li>Shop DC</li>
                    <li>Shop DC COllectibles</li>
                </ul>
            </div>
            <div>
                <h3>DC COMICS</h3>
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
                <h3>SITES</h3>
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
        <div id="foot-bar">
            <div id="foot-social" class="container">
                <div id="foot-left">
                    SIGN-UP NOW!
                </div>
                <div id="foot-right">
                    <div id="follow">FOLLOW US</div>
                    <div id="social">
                        <div>
                            <img src="../assets/img/footer-facebook.png" alt="facebook">
                            <img src="../assets/img/footer-twitter.png" alt="twitter">
                            <img src="../assets/img/footer-youtube.png" alt="youtube">
                            <img src="../assets/img/footer-pinterest.png" alt="pinterest">
                            <img src="../assets/img/footer-periscope.png" alt="periscope">
                        </div>
                    </div>
                </div>
            </div>
        </div>

    </footer>
</template>

<style lang="scss">
@use 'styles/general' as *;
@use 'styles/partials/mixins' as *;
@use 'styles/partials/variables' as *;

footer {
    background-image: url(../assets/img/footer-bg.jpg);
    height: 100%;

    #content-info {
        display: flex;
        justify-content: flex-start;
        gap: 25px;
        color: $white-font;
        padding: 20px 0;
        position: relative;
        overflow: hidden;

        h3 {
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

