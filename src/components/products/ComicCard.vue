<script>
export default {
    data() {
        return {

        }
    },
    props: {
        product: Object
    }
}
</script>

<template>
    <div class="card">
        <img :src="product.thumb" :alt="product.series">
        <h3>{{ product.series }}</h3>
    </div>
</template>

<style lang="scss" scoped>
.card {
    padding: 20px;

    img {
        display: block;
    }

    h3 {
        color: white;
        font-size: 14px;
        margin-top: 10px;
    }
}
</style>