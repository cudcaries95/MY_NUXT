<template>
    <div class="grid grid-cols-2 gap-20">
        <div>
            <img :src="product.image" alt="product img" class="h-full w-auto pl-16">
        </div>
        <div class="flex flex-col justify-center">
            <h1 class="font-robotoslab text-4xl font-bold mb-5">Exclusive Offer</h1>
            <p class="font-poppins text-xl mb-9">Open for sale at extremely preferential prices until October 5, 2023</p>
            <div class="flex gap-7 mb-9">
                <button class="h-20 w-20 border bg-white">
                    <p class="text-2xl font-poppins font-semibold">06</p>
                    <p class="text-sm font-poppins">Days</p>
                </button>
                <button class="h-20 w-20 border bg-white">
                    <p class="text-2xl font-poppins font-semibold">18</p>
                    <p class="text-sm font-poppins">Hours</p>
                </button>
                <button class="h-20 w-20 border bg-white">
                    <p class="text-2xl font-poppins font-semibold">48</p>
                    <p class="text-sm font-poppins">Mins</p>
                </button>
            </div>
            <p class="">                
                <NuxtLink to="/products/14">
                    <button class="bg-green-800 text-white border-2 w-60 h-16 text-xl font-poppins">BUY NOW</button>
                </NuxtLink>
            </p>
        </div>
    </div>
</template>

<script setup>
    const { product } = defineProps(['product'])
</script>

<style scoped>
    img {
        height: 516px;
    }
</style>