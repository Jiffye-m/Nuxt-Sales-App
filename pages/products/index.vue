<template>
    <div>

        <div class="grid grid-cols-4 gap-5">
            
                <div  v-for="p in products" :key="p">
                  <ProductCard :product="p"/>
                </div>
            
            
        </div>

    </div>
</template>

<script setup>

definePageMeta({
    layout: 'products'
})

//fetch products
const { data: products } = await useFetch('https://api.escuelajs.co/api/v1/products')

</script>

<style scoped>

</style>