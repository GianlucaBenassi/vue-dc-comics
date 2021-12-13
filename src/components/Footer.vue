<template>

    <footer>

        <!-- shop footer section -->
        <div class="shop">
            <div class="container">

                <div class="box">
                    <a href="#">
                        <img src="..\assets\img\buy-comics-digital-comics.png" alt="Digital comics">
                        <span>digital comics</span>
                    </a>
                </div>

                <div class="box">
                    <a href="#">
                        <img src="..\assets\img\buy-comics-merchandise.png" alt="DC merchandise">
                        <span>dc merchandise</span>
                    </a>
                </div>

                <div class="box">
                    <a href="#">
                        <img src="..\assets\img\buy-comics-subscriptions.png" alt="Subscription">
                        <span>subscription</span>
                    </a>
                </div>

                <div class="box">
                    <a href="#">
                        <img src="..\assets\img\buy-comics-shop-locator.png" alt="Comic shop locator">
                        <span>comic shop locator</span>
                    </a>
                </div>

                <div class="box">
                    <a href="#">
                        <img src="..\assets\img\buy-dc-power-visa.svg" alt="DC power VISA">
                        <span>dc power visa</span>
                    </a>
                </div>

            </div>
        </div>

        <!-- footer links -->
        <div class="links">
            <div class="container">

            </div>
        </div>

        <!-- socials -->
        <div class="social">
            <div class="container">
                
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

@import '../assets/style/partials/variables.scss';

.shop {
    background-color: $mainColor;
    padding: 50px 0;

    .container {
        display: flex;
        flex-wrap: wrap;
        justify-content: space-around;
    
        .box a {
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
            }
        }
    }
}

</style>