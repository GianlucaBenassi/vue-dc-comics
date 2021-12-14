<template>

    <header>
        <div class="container">

            <a href="#" class="logo">
                <img src="..\..\assets\img\dc-logo.png" alt="header logo">
            </a>

            <nav>
                <ul :class="{close : closeMenu}">
                    <li><a href="#">characters</a></li>
                    <li><a href="#" class="active">comics</a></li>
                    <li><a href="#">movies</a></li>
                    <li><a href="#">tv</a></li>
                    <li><a href="#">games</a></li>
                    <li><a href="#">collectibles</a></li>
                    <li><a href="#">videos</a></li>
                    <li><a href="#">fans</a></li>
                    <li><a href="#">news</a></li>
                    <li><a href="#">shop</a></li>
                </ul>
                <div @click="openMenu()">
                    <i class="fas fa-bars"></i>
                </div>
            </nav>

        </div>
    </header>

</template>

<script>
export default {
    name: 'Header',
    data() {
        return {
            closeMenu: false
        }
    },
    methods: {
        onResize() {
            if (window.innerWidth <= 1200) {
                this.closeMenu = true;
            } else {
                this.closeMenu = false;
            }
        },
        openMenu() {
            this.closeMenu = !this.closeMenu;
        }
    },
    mounted() {
        this.onResize()
        window.addEventListener('resize', this.onResize, { passive: true })
    }
}
</script>

<style lang="scss" scoped>

@import '../../assets/style/partials/variables.scss';

header {
    height: 100px;
    position: relative;

    @media screen and (max-width: 1200px) {
        padding: 0 20px;
    }
}

.close {
    display: none;
}

.container {
    height: 100%;
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.logo {
    height: 80%;

    img {
        height: 100%;
    }
}

nav {
    height: 100%;

    ul {
        height: 100%;
        display: flex;
        align-items: center;

        li {
            height: 100%;
            margin-left: 20px;
            line-height: 100px;

            a {
                height: 100%;
                color: #000;
                font-size: 14px;
                font-weight: bold;
                text-transform: uppercase;
                display: inline-block;

                &.active, &:hover {
                    color: $mainColor;
                    border-bottom: 5px solid $mainColor;
                }
            }
        }
    }

    .fa-bars {
        font-size: 25px;
        display: none;
        cursor: pointer;
    }

    @media screen and (max-width: 1200px) {
        & {
            display: flex;
            align-items: center;

            ul {
                width: 100%;
                height: initial;
                background-color: #eee;
                position: absolute;
                left: 0;
                top: 100px;
                flex-direction: column;
                align-items: flex-start;
                z-index: 9999;

                li {
                    line-height: initial;
                    margin: 10px 0 10px 20px;

                    a {
                        padding: 10px 0;

                        &.active, &:hover {
                            border-bottom: none;
                        }   
                    }

                }
            }

            .fa-bars {
                display: block;
            }
        }


    }
}

</style>