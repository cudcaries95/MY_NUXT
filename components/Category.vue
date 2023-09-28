<template>
    <div>
        <div class="card h-80 w-auto flex justify-items-center">
            <img :src="product.image" alt="product thumb" class="max-w-auto max-h-80">
        </div>
        <div class="">
            <p class="font-poppins font-semibold text-gray-500 mt-8 truncate text-center">{{ product.title }}</p>
            <p class="font-poppins text-gray-500 mt-2 truncate text-center">{{ product.category }} | ${{ product.price }}</p>
        </div>
    </div>
</template>

<script setup>
const { product } = defineProps(['product'])
</script>

<style scoped></style>