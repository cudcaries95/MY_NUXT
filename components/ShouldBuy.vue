<template>
    <div>
        <div class="card flex justify-items-center">
            <img :src="product.image" alt="product thumb" class="h-full w-auto">
        </div>
        <div class="mt-5">
            <p class="font-poppins font-semibold text-2xl text-gray-500 text-center mb-2">{{ product.category }}</p>
            <p class="font-poppins text-xl text-gray-500">{{ product.description }}</p>
        </div>
    </div>
</template>

<script setup>
const { product } = defineProps(['product'])
</script>

<style scoped>
    img {
        height: 490px;
    }
</style>