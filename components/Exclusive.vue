<template>
    <div class="grid grid-cols-2 gap-10">
        <div class="p-7">
            <img :src="product.image" alt="product img" class="mx-auto my-7 max-h-full max-w-auto rounded-3xl">
        </div>
        <div class="p-7 flex flex-col justify-center">
            <h1 class="text-4xl my-7 font-bold">Exclusive Offer</h1>
            <p class="text-2xl my-7">Open for sale at extremely preferential prices until October 5, 2023</p>
            <p class="mt-5 mb-5">                
                <NuxtLink to="/products/14">
                    <button class="bg-green-800 text-white border-2 px-4 py-4 text-2xl">BUY NOW</button>
                </NuxtLink>
            </p>
        </div>
    </div>
</template>

<script setup>
    const { product } = defineProps(['product'])
</script>

<style scoped>

</style>