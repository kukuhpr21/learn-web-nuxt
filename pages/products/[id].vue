<template>
    <ProductDetails :product="product"/>
</template>

<script setup>
const { id } = useRoute().params
const uri = 'https://fakestoreapi.com/products/' + id

definePageMeta({
    layout: 'products',
})

// fetch the product detail
const { data: product } = await useFetch(uri, {key: id})
</script>

<style scoped>

</style>