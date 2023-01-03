<template>
    <div>
        <header class="bg-slate-800 py-4 mb-12">
            <div class="container">
                <nav class="flex align-middle justify-between">
                <div class="w-25 text-3xl font-extrabold text-white">
                    <NuxtLink to="/">Nuxt</NuxtLink></div>
                    <ul class="flex text-white justify-between gap-6">
                        <li><NuxtLink to="/">Home</NuxtLink></li>
                        <li><NuxtLink to="/about">About us</NuxtLink></li>
                        <li><NuxtLink to="/products">Products</NuxtLink></li>
                    </ul>
                </nav>
            </div>
        </header>

        <div>
            <slot />
        </div>

        <footer class="bg-slate-800 py-4 text-white mt-12">
            <div class="container">
                <p class="text-center py-4">Copyright &nbsp; Md Ayub Ali</p>
            </div>
        </footer>
    </div>
</template>

<script setup>

</script>

<style scoped>
    .router-link-exact-active{
        color: green;
    }
</style>