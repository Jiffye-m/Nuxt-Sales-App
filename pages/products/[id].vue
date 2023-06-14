<template>
    <div>

        <ProductDetails v-bind:product="product"/>

    </div>
</template>

<script setup>

const { id } = useRoute().params

const uri = 'https://api.escuelajs.co/api/v1/products/' + id

//fetch the product
const { data: product } = await useFetch(uri)

definePageMeta({
    layout: 'products'
})


</script>

<style scoped>

</style>