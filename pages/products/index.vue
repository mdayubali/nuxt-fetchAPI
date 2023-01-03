<template>
    <div>
        <div class="container">
            <div class="grid grid-cols-4 gap-5">
            <div v-for="p in products">
                <img :src="p.thumbnailUrl" alt="title">
                <NuxtLink :to="`/products/${p.id}`">{{ p.title }}</NuxtLink>
            </div>
        </div>
        </div>
    </div>
</template>

<script setup>
    definePageMeta({
        layout:'products'
    })
   // fetch products
    const { data: products } = await useFetch('https://jsonplaceholder.typicode.com/photos?_page=1&_limit=48')
    console.log(products)
</script>

<style lang="scss" scoped>

</style>