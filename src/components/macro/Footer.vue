<template>

    <footer>

        <!-- shop footer section -->
        <div class="shop">
            <div class="container">

                <div class="box">
                    <a href="#">
                        <img src="..\..\assets\img\buy-comics-digital-comics.png" alt="Digital comics">
                        <span>digital comics</span>
                    </a>
                </div>

                <div class="box">
                    <a href="#">
                        <img src="..\..\assets\img\buy-comics-merchandise.png" alt="DC merchandise">
                        <span>dc merchandise</span>
                    </a>
                </div>

                <div class="box">
                    <a href="#">
                        <img src="..\..\assets\img\buy-comics-subscriptions.png" alt="Subscription">
                        <span>subscription</span>
                    </a>
                </div>

                <div class="box">
                    <a href="#">
                        <img src="..\..\assets\img\buy-comics-shop-locator.png" alt="Comic shop locator">
                        <span>comic shop locator</span>
                    </a>
                </div>

                <div class="box">
                    <a href="#">
                        <!-- <img src="..\..\assets\img\buy-comics-shop-locator.png" alt="Comic shop locator"> -->
                        <img src="..\..\assets\img\buy-dc-power-visa.svg" alt="DC power VISA">
                        <span>dc power visa</span>
                    </a>
                </div>

            </div>
        </div>

        <!-- footer links -->
        <div class="links">
            <div class="container">

                <div class="left">

                    <div class="col">
                        <h4>dc comics</h4>
                        <ul>
                            <li><a href="#">Characters</a></li>
                            <li><a href="#">Comics</a></li>
                            <li><a href="#">Movie</a></li>
                            <li><a href="#">TV</a></li>
                            <li><a href="#">Games</a></li>
                            <li><a href="#">Videos</a></li>
                            <li><a href="#">News</a></li>
                        </ul>

                        <h4>shop</h4>
                        <ul>
                            <li><a href="#">Shop DC</a></li>
                            <li><a href="#">Shop DC Collectibles</a></li>
                        </ul>

                    </div>

                    <div class="col">
                        <h4>dc</h4>
                        <ul>
                            <li><a href="#">Terms Of Use</a></li>
                            <li><a href="#">Provacy policy (New)</a></li>
                            <li><a href="#">Ad Choices</a></li>
                            <li><a href="#">Advertising</a></li>
                            <li><a href="#">Jobs</a></li>
                            <li><a href="#">Subscriptions</a></li>
                            <li><a href="#">Talent Workshops</a></li>
                            <li><a href="#">CPSC Certificates</a></li>
                            <li><a href="#">Ratings</a></li>
                            <li><a href="#">Shop Help</a></li>
                            <li><a href="#">Contact Us</a></li>
                        </ul>
                    </div>

                    <div class="col">
                        <h4>sites</h4>
                        <ul>
                            <li><a href="#">DC</a></li>
                            <li><a href="#">MAD Magazine</a></li>
                            <li><a href="#">DC Kids</a></li>
                            <li><a href="#">DC Universe</a></li>
                            <li><a href="#">DC Power Visa</a></li>
                        </ul>
                    </div>

                </div>

                <div class="right">
                    <!-- only background image -->
                </div>

            </div>
        </div>

        <!-- socials -->
        <div class="social">
            <div class="container">

                <a href="#" class="sing-up">sing-up now!</a>

                <div class="icons">
                    <a href="#"><span>follow us</span></a>
                    <a href="#"><img src="..\..\assets\img\footer-facebook.png" alt="facebook"></a>
                    <a href="#"><img src="..\..\assets\img\footer-twitter.png" alt="twitter"></a>
                    <a href="#"><img src="..\..\assets\img\footer-youtube.png" alt="youtube"></a>
                    <a href="#"><img src="..\..\assets\img\footer-pinterest.png" alt="pinterest"></a>
                    <a href="#"><img src="..\..\assets\img\footer-periscope.png" alt="peroscope"></a>
                </div>

            </div>
        </div>

    </footer>

</template>

<script>
export default {
    name: 'Footer'
}
</script>

<style lang="scss" scoped>

@import '../../assets/style/partials/variables.scss';

.shop {
    background-color: $mainColor;
    padding: 50px 0;

    .container {
        display: flex;
        flex-wrap: wrap;
        justify-content: space-around;
    
        .box{
            min-width: 200px;


            a {
                margin: 20px 0;
                display: flex;
                align-items: center;

                img {
                    max-height: 50px;
                }

                span {
                    color: #fff;
                    text-transform: uppercase;
                    white-space: nowrap;
                    margin-left: 15px;
                    transition: all .3s;
                }
            }

            &:hover a span {
                color: $secondColor;
            }

        }
    }
}

.links {
    background-image: url('../../assets/img/footer-bg.jpg');
    background-size: cover;
    background-position: center;

    .container {
        display: flex;
        justify-content: space-between;

        .left {
            display: flex;

            .col {
                padding: 35px 25px 35px 0;

                h4 {
                    color: #fff;
                    text-transform: uppercase;
                    font-size: 18px;
                    padding: 20px 0;
                }

                ul li a {
                    color: #8f8f8f;
                    font-size: 14px;
                    margin: 3px 0;
                    display: inline-block;

                    &:hover {
                        color: #fff;
                        text-decoration: underline;
                    }
                }
                
            }

            @media screen and (max-width: 520px) {
                flex-direction: column;
                margin-left: 40px;

                .col {
                    padding: 10px 0;
                }
            }
        }

        .right {
            width: 50%;
            background-image: url('../../assets/img/dc-logo-bg.png');
            background-size: cover;
            background-position: center;

            @media screen and (max-width: 1200px) {
                width: 40%;
            }

            @media screen and (max-width: 720px) {
                display: none;
            }
        }

    }
    
}

.social {
    background-color: #303030;

    .container {
        padding: 30px 0;
        display: flex;
        justify-content: space-between;

        .sing-up {
            color: #fff;
            text-transform: uppercase;
            border: 2px solid $mainColor;
            padding: 10px;
        }

        .icons {
            display: flex;
            align-items: center;

            a {
                color: $mainColor;
                text-transform: uppercase;
                font-size: 18px;
                font-weight: bold;
                margin-left: 10px;
            }
        }

        @media screen and (max-width: 520px) {
            flex-direction: column;
            align-items: center;

            .sing-up {
                margin-bottom: 20px;
            }
        }
    }
}

</style>