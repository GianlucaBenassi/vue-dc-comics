<template>

    <header>
        <div class="container">

            <div class="logo">
                <img src="..\..\assets\img\dc-logo.png" alt="header logo">
            </div>

            <nav>
                <ul>
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
            </nav>

        </div>
    </header>

</template>

<script>
export default {
    name: 'Header'
}
</script>

<style lang="scss" scoped>

@import '../../assets/style/partials/variables.scss';

header {
    height: 100px;
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
            line-height: 100PX;

            a {
                color: #000;
                font-size: 14px;
                font-weight: bold;
                text-transform: uppercase;
                height: 100%;
                display: inline-block;

                &.active, &:hover {
                    color: $mainColor;
                    border-bottom: 5px solid $mainColor;
                }
            }
        }
    }
}

</style>