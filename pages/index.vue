<template> 
<div class="bg-teal-50">
    <div class="mb-10">
        <div class="bg-teal-50 rounded-2xl mb-1">
            <HomePro :product = "product7"/>
        </div>
    </div>
    <div class="mt-40">
        <div>
            <h2 class="text-center mb-5 text-4xl">Best Selling</h2>
            <p class="text-center mb-5">Bringing you great experiences at extremely shocking prices</p>
            
        </div>  
        <div class="grid grid-cols-3 gap-x-6 mx-auto">
            <div v-for="p in products">
                <BestSell :product="p"/>            
            </div>
        </div>
        <p class="grid justify-items-center mt-5 mb-5 mx-auto">
            <NuxtLink to="/products" class="btn">See all</NuxtLink>
        </p>      
    </div> 
    <div class="mt-40">
        <div>            
            <h2 class="text-center mb-5 text-4xl">CATEGORIES</h2>
            <ul class="mx-auto mt-16 mb-16 flex justify-center gap-8 text-2xl">                  
                <li><NuxtLink to="/">JEWELERY</NuxtLink></li>
                <li><NuxtLink to="/">ELECTRONICS</NuxtLink></li>
                <li><NuxtLink to="/">MEN'S CLOTHING</NuxtLink></li>
                <li><NuxtLink to="/">WOMEN'S CLOTHING</NuxtLink></li>
            </ul>          
            </div>  
            <div class="grid grid-cols-4 gap-x-6 mx-auto">
                <div v-for="p in productoe" class="p-5">
                    <ProductCard :product="p"/>            
                </div>
            </div>             
    </div> 
    <div class="my-10">
        <div class="bg-white rounded-2xl mb-1">
            <Exclusive :product = "product5"/>
        </div>
    </div>
    <div class="grid grid-cols-4  bg-lime-400 h-auto max-w-full">
        <div class="p-12">
            <h1 class="font-bold text-3xl">MY NUXT</h1>
            <h2 class="text-xl">Social Media</h2>
            <div class="flex">
                <NuxtLink to="/"><Icon name="uil:github" color="black"/></NuxtLink>
                <NuxtLink to="/"><Icon name="uil:twitter" color="black"/></NuxtLink>
                <NuxtLink to="/"><Icon name="uil:facebook" color="black"/></NuxtLink>
            </div>            
        </div>
        <div class="p-12">
            <h1 class="font-bold text-2xl">SHOP</h1>
            <h2 class="text-xl">Products</h2>
            <h2 class="text-xl">Overview</h2>
            <h2 class="text-xl">Pricing</h2>
            <h2 class="text-xl">Releases</h2>
        </div>
        <div class="p-12">
            <h1 class="font-bold text-2xl">COMPANY</h1>
            <h2 class="text-xl">About Us</h2>
            <h2 class="text-xl">Contact</h2>
            <h2 class="text-xl">News</h2>
            <h2 class="text-xl">Support</h2>
        </div>
        <div class="p-12">
            <h1 class="font-bold text-2xl">STAY UP TO DATE</h1>
            <h2 class="text-xl">Button</h2>
        </div>
    </div>
</div>
    
    
</template>

<script setup>
    const { data: product7 } = await useFetch('https://fakestoreapi.com/products/7')

    const { data: product5 } = await useFetch('https://fakestoreapi.com/products/5')

    const { data: products } = await useFetch('https://fakestoreapi.com/products?limit=3')

    const { data: productoj} = await useFetch('https://fakestoreapi.com/products/category/jewelery')

    const { data: productoe} = await useFetch('https://fakestoreapi.com/products/category/electronics')

    const { data: productom} = await useFetch(`https://fakestoreapi.com/products/category/men's clothing`)

    const { data: productow} = await useFetch(`https://fakestoreapi.com/products/category/women's clothing`)
    
</script>

<style scoped>
</style>