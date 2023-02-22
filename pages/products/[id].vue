<template>
    <head>
        <Title>Nuxt Kukuh | {{ product.title }}</Title>
        <Meta name="description" :content="product.description"/>
    </head>
    <ProductDetails :product="product"/>
</template>

<script setup>
const { id } = useRoute().params
const uri = 'https://fakestoreapi.com/products/' + id

// fetch the product detail
const { data: product } = await useFetch(uri, {key: id})

// handle error if product value is empty
if (!product.value) {
    throw createError({ statusCode: 404, statusMessage: 'Product Not Found', fatal: true})
}

definePageMeta({
    layout: 'products',
})
</script>

<style scoped>

</style>