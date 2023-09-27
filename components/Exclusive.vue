<template>
    <div class="grid grid-cols-2 gap-10">
        <div class="p-7">
            <p></p>
            <img :src="product.image" alt="product img" class="mx-auto my-7 max-w-sm rounded-3xl">
        </div>
        <div class="p-7 flex flex-col justify-center">
            <h2 class="text-4xl my-7 font-bold">Exclusive Offer</h2>
            <p class="text-4xl my-7">Open for sale at extremely preferential prices until October 5, 2023</p>
            <p class="mt-5 mb-5 mx-auto">
                <NuxtLink to="/products/5" class="btn">BUY NOW</NuxtLink>
            </p>
        </div>
    </div>
</template>

<script setup>
    const { product } = defineProps(['product'])
</script>

<style scoped>

</style>