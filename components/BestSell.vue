<template>
    <div>
        <div class="card py-10 h-96 flex justify-items-center">
            <img :src="product.image" alt="product thumb" class="mx-auto max-w-auto max-h-96">
        </div>
        <div class="">
            <p class="text-gray-500 m-4 truncate text-center font-poppins font-semibold">{{ product.title }}</p>
            <p class="text-gray-500 m-4 truncate text-center font-poppins font-medium">{{ product.category }} | ${{ product.price }}</p>
        </div>
    </div>
</template>

<script setup>
const { product } = defineProps(['product'])
</script>

<style scoped></style>