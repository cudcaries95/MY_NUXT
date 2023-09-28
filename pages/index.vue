<template>
    <div>
        <div class="bg-emerald-100">
            <nav class="grid grid-cols-3 mx-auto p-10 ">
                <NuxtLink to="/" class="font-bold italic text-4xl">MY NUXT</NuxtLink>
                <ul class="flex gap-10 justify-center">
                    <li>
                        <NuxtLink to="/" class="text-2xl">HOME</NuxtLink>
                    </li>
                    <li>
                        <NuxtLink to="/about" class="text-2xl">SHOP</NuxtLink>
                    </li>
                    <li>
                        <NuxtLink to="/products" class="text-2xl">FUTURES</NuxtLink>
                    </li>
                    <li>
                        <NuxtLink to="/products" class="text-2xl">CONTACT</NuxtLink>
                    </li>
                </ul>
                <ul class="flex gap-4 justify-end">
                    <NuxtLink to="/">
                        <Icon class="h-8 w-20" name="uil:bell" color="black" />
                    </NuxtLink>
                    <NuxtLink to="/"><button class="border-black border-2 px-4 text-2xl">LOGIN</button></NuxtLink>
                </ul>
            </nav>
        </div>
        <div class="mb-20">
            <div class="bg-emerald-100">
                <HomePro :product="product7" />
            </div>
        </div>
        <div class="mt-40 px-10">
            <div>
                <h2 class="text-center mb-5 text-4xl">Best Selling</h2>
                <p class="text-center mb-5">Bringing you great experiences at extremely shocking prices</p>
            </div>
            <div class="grid grid-cols-3 gap-x-6 mx-auto">
                <div v-for="p in products">
                    <BestSell :product="p" />
                </div>
            </div>
            <div class="flex justify-center mt-10">
                <NuxtLink to="/products">
                    <button class="border-black border-2 px-4 py-2 text-2xl w-48">See all
                        <Icon name="uil:arrow-right" color="black" />
                    </button>
                </NuxtLink>
            </div>
        </div>
        <div class="mt-40 mb-20 px-10">
            <div>
                <h2 class="text-center mb-5 text-4xl">CATEGORIES</h2>
                <ul class="mx-auto mt-16 mb-16 flex justify-center gap-8 text-2xl">
                    <li>
                        <NuxtLink to="/">JEWELERY</NuxtLink>
                    </li>
                    <li>
                        <NuxtLink to="/">ELECTRONICS</NuxtLink>
                    </li>
                    <li>
                        <NuxtLink to="/">MEN'S CLOTHING</NuxtLink>
                    </li>
                    <li>
                        <NuxtLink to="/">WOMEN'S CLOTHING</NuxtLink>
                    </li>
                </ul>
            </div>
            <div class="grid grid-cols-4 gap-x-6 mx-auto">
                <div v-for="p in productoe" class="p-5">
                    <Category :product="p" />
                </div>
            </div>
        </div>
        <div class="px-10">
            <div class="bg-emerald-100 rounded-2xl mb-1">
                <Exclusive :product="product14" />
            </div>
        </div>
        <div class="mt-40 px-10">
            <div>
                <h2 class="text-center mb-5 text-4xl">You should buy!</h2>
                <p class="text-center mb-5">Items that should be in your shopping cart</p>
            </div>
            <div class="grid grid-cols-3 gap-x-6 mx-auto">
                <div v-for="p in productoj">
                    <ShouldBuy :product="p" />
                </div>
            </div>
        </div>
        <div class="my-40 px-10">
            <div>
                <h2 class="text-center mb-20 text-4xl">Feedback Corner</h2>
            </div>
            <div class="grid grid-cols-3 gap-x-6 mx-auto">
                <div class="border-black border-2 p-4 text-2xl">
                    <Icon name="uil:feedback" />
                    <h1 class="py-4 font-bold">Adam Smit</h1>
                    <h2>The customer experience was exceptional from start to finish. The website is user-friendly, the
                        checkout process was smooth, and the clothes I ordered fit perfectly. I'm beyond satisfied!</h2>
                </div>
                <div class="border-black border-2 p-4 text-2xl">
                    <Icon name="uil:feedback" />
                    <h1 class="py-4 font-bold">Lyly Anna</h1>
                    <h2>I absolutely love the quality and style of the clothing I purchased from this website. customer
                        service was outstanding, and I received my order quickly. Highly recommended!</h2>
                </div>  
                <div class="border-black border-2 p-4 text-2xl">
                    <Icon name="uil:feedback" />
                    <h1 class="py-4 font-bold">Hor Walk</h1>
                    <h2>I had a great experience shopping on this website. The clothes I bought are fashionable and
                        comfortable. Highly satisfied!</h2>
                </div>
            </div>
        </div>
        <div class="grid grid-cols-4 auto-cols-max bg-green-800 h-auto max-w-full text-white">
            <div class="p-12">
                <h1 class="font-bold text-3xl pb-3">MY NUXT</h1>
                <h2 class="text-xl pb-3">Social Media</h2>
                <div class="flex">
                    <NuxtLink class="mr-5" to="/">
                        <Icon class="text-4xl" name="uil:github" color="white" />
                    </NuxtLink>
                    <NuxtLink class="mr-5" to="/">
                        <Icon class="text-4xl" name="uil:twitter" color="white" />
                    </NuxtLink>
                    <NuxtLink class="mr-5"  to="/">
                        <Icon class="text-4xl" name="uil:facebook" color="white" />
                    </NuxtLink>
                </div>
            </div>
            <div class="p-12">
                <h1 class="font-bold text-2xl pb-3">SHOP</h1>
                <h2 class="text-xl pb-3">Products</h2>
                <h2 class="text-xl pb-3">Overview</h2>
                <h2 class="text-xl pb-3">Pricing</h2>
                <h2 class="text-xl pb-3">Releases</h2>
            </div>
            <div class="p-12">
                <h1 class="font-bold text-2xl pb-3">COMPANY</h1>
                <h2 class="text-xl pb-3">About Us</h2>
                <h2 class="text-xl pb-3">Contact</h2>
                <h2 class="text-xl pb-3">News</h2>
                <h2 class="text-xl pb-3">Support</h2>
            </div>
            <div class="p-12">
                <h1 class="font-bold text-2xl pb-3">STAY UP TO DATE</h1>
                <h2 class="flex pb-3"><input type="text" placeholder="Enter your email"><button class="bg-lime-300 border-2 text-black">SUBMIT</button></h2>
            </div>
        </div>
        <div class="bg-green-800 h-auto max-w-full text-white">
            <div class="p-12 flex justify-between">
                <hr class="my-auto w-2/3"/>
                <p class="text-xl">Terms</p>
                <h2 class="text-xl ">Privacy</h2>
                <h2 class="text-xl ">Cookies</h2>              
                              
            </div>
        </div>
    </div>
</template>

<script setup>

const { data: product7 } = await useFetch('https://fakestoreapi.com/products/7')

const { data: product14 } = await useFetch('https://fakestoreapi.com/products/14')

const { data: products } = await useFetch(`https://fakestoreapi.com/products/category/men's clothing?limit=3`)

const { data: productoj } = await useFetch(`https://fakestoreapi.com/products/category/women's clothing?limit=3&sort=desc`)

const { data: productoe } = await useFetch('https://fakestoreapi.com/products?limit=8')

const { data: productom } = await useFetch(`https://fakestoreapi.com/products/category/men's clothing`)

const { data: productow } = await useFetch(`https://fakestoreapi.com/products/category/women's clothing`)

</script>

<style scoped></style>