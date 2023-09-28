<template>
    <div class="grid grid-cols-2 gap-10">        
        <div class="flex flex-col justify-center">
            <h2 class="font-rufina font-bold text-7xl my-6">{{ product.title }}</h2>
            <p class="font-poppins font-medium text-2xl my-6">{{ product.description }}</p>
            <p >                
                <NuxtLink to="/products/7">
                    <button class="font-poppins bg-green-800 text-white border text-xl w-56 h-16">EXPLORE NOW</button>
                </NuxtLink>
            </p>
        </div>
        <div class="pb-20">
            <p></p>
            <img :src="product.image" alt="product img" class="">
        </div>
    </div>
</template>

<script setup>
    const { product } = defineProps(['product'])
</script>

<style scoped>
    img {
        width: 449x;
        height: 621px;
        border-radius: 20% 5% 20% 10%;
    }
</style>