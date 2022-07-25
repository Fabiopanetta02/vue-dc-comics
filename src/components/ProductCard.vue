<template>
    <div class="games-card">
        <img :src="productSrc" :alt=" productTitle">
        <h3>{{ productTitle.toUpperCase() }}</h3>
    </div>
</template>

<script>
export default {
    name: 'ProductCard',
    props: {
        productTitle: String,
        productSrc: String
    }
}
</script>

<style lang="scss" scoped>
.games-card{
    flex-basis: calc(100% / 6);

    img{
        height: 192px;
        width: 192px;
        object-fit: cover;
        object-position: top;
        margin-bottom: 10px;
    }

    h3{
        margin-bottom: 40px;
        width: 192px;
    }
}

</style>