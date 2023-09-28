<template>
    <div>
        <div class="card py-10 h-96 flex justify-items-center">
            <img :src="product.image" alt="product thumb" class="max-w-auto max-h-80">
        </div>
        <div class="">
            <p class="font-bold text-gray-500 m-4 truncate text-center">{{ product.title }}</p>
            <p class="font-bold text-gray-500 m-4 truncate text-center">{{ product.category }} | ${{ product.price }}</p>
        </div>
    </div>
</template>

<script setup>
const { product } = defineProps(['product'])
</script>

<style scoped></style>