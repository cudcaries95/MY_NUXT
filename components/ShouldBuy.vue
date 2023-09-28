<template>
    <div>
        <div class="card py-10">
            <img :src="product.image" alt="product thumb" class="mx-auto max-w-auto max-h-96">
        </div>
        <div class="">
            <p class="font-bold text-gray-500 m-4 truncate text-center">{{ product.category }}</p>
            <p class="font-bold text-gray-500 m-4 ">{{ product.description }}</p>
        </div>
    </div>
</template>

<script setup>
const { product } = defineProps(['product'])
</script>

<style scoped></style>