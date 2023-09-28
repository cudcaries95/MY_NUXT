<template>
    <div class="grid grid-cols-2 gap-10">        
        <div class="p-10 flex flex-col justify-center">
            <h2 class="text-4xl my-7">{{ product.title }}</h2>
            <p class="text-4xl my-7">Price - ${{ product.price }}</p>
            <h3 class="font-bold border-b-2 mb-4 pb-2 text-2xl">Product description:</h3>
            <p class="mb-7 text-2xl">{{ product.description }}</p>
            <p class="mt-5 mb-5">                
                <NuxtLink to="/products/7">
                    <button class="bg-green-800 text-white border-2 px-4 py-4 text-2xl">EXPLORE NOW</button>
                </NuxtLink>
            </p>
        </div>
        <div class="p-10">
            <p></p>
            <img :src="product.image" alt="product img" class="my-7 max-w-lg rounded-bl-3xl rounded-tr-3xl">
        </div>
    </div>
</template>

<script setup>
    const { product } = defineProps(['product'])
</script>

<style scoped>

</style>