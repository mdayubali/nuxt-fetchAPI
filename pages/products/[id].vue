<template>
    <div>
        <div class="container">
            <h2 class="text-2xl font-semibold">Product details {{ id }}</h2>
        </div>
    </div>
</template>

<script setup>
const {id} = useRoute().params;
definePageMeta({
    layout: 'products'
})


</script>

<style scoped>

</style>