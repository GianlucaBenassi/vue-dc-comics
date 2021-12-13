<template>
    <main>
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

@import '../assets/style/partials/variables.scss';

main {
    color: #fff;
    font-size: 30px;
    background-color: $secondColor;
    padding: 50px 0;
}

</style>