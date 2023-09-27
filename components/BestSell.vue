<template>
    <div class="card text-center rounded-bl-3xl rounded-tr-3xl">
        <img :src="product.image" alt="product thumb" class="max-w-xs max-h-60 mx-auto">
        <p class="font-bold text-gray-500 m-4 truncate">{{ product.title }}</p>
        <p class="font-bold text-gray-500 m-4 truncate">{{ product.categories }}</p>
        <p class="font-bold text-gray-500 m-4 truncate">{{ product.price }}</p>
    </div>
</template>

<script setup>
    const { product } = defineProps(['product'])
</script>

<style scoped>
</style>