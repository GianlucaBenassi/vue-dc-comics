<template>
    <main>

        <div class="jumbo">
            <img src="../../assets/img/jumbotron.jpg" alt="">
        </div>

        <div class="container">
            <span>--&gt; Content goes here 	&lt;--</span>
        </div>
    </main>
</template>

<script>
export default {
    name: 'Main'
}
</script>

<style lang="scss" scoped>

@import '../../assets/style/partials/variables.scss';

main {
    color: #fff;
    font-size: 30px;
    background-color: $secondColor;
}

.jumbo {
    height: 400px;

    img {
        width: 100%;
        height: 100%;
        object-fit: cover;
        object-position: top;
    }
}

</style>