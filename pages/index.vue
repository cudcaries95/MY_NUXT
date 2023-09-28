<template>
    <div>
        <div class="bg-emerald-100">
            <nav class="flex m-auto px-36 py-12 ">
                <NuxtLink to="/" class="font-serif font-bold text-4xl m-auto justify-start">Nuxt</NuxtLink>
                <ul class="flex gap-10 m-auto justify-center">
                    <li>
                        <NuxtLink to="/" class="text-xl font-poppins">HOME</NuxtLink>
                    </li>
                    <li>
                        <NuxtLink to="/about" class="text-xl font-poppins">SHOP</NuxtLink>
                    </li>
                    <li>
                        <NuxtLink to="/products" class="text-xl font-poppins">FUTURES</NuxtLink>
                    </li>
                    <li>
                        <NuxtLink to="/products" class="text-xl font-poppins">CONTACT</NuxtLink>
                    </li>
                </ul>
                <ul class="flex gap-4 m-auto justify-stretch">
                    <NuxtLink class="place-self-center" to="/">
                        <Icon class="h-8 w-8 " name="uil:bell" color="black" />
                    </NuxtLink>
                    <NuxtLink to="/"><button class="w-32 h-11 font-poppins border-black border px-4 text-xl">LOGIN</button>
                    </NuxtLink>
                </ul>
            </nav>
        </div>
        <div class="px-36 bg-emerald-100 pt-28">
            <div class="bg-emerald-100">
                <HomePro :product="product7" />
            </div>
        </div>
        <div class="mt-24 px-36">
            <div>
                <h2 class="text-center mb-6 text-5xl font-robotoslab">Best Selling</h2>
                <p class="text-center mb-6 text-xl font-poppins">Bringing you great experiences at extremely shocking prices
                </p>
            </div>
            <div class="grid grid-cols-3 gap-x-6 mx-auto mt-11">
                <div v-for="p in products">
                    <BestSell :product="p" />
                </div>
            </div>
            <div class="flex justify-center mt-16 text-center">
                <NuxtLink to="/products">
                    <button class="border-black border-2 px-4 py-2 font-poppins text-xl w-48">See all
                        <Icon name="uil:arrow-right" color="black" />
                    </button>
                </NuxtLink>
            </div>
        </div>
        <div class="mt-40 px-36">
            <div>
                <h2 class="text-center text-5xl font-robotoslab">Categories</h2>
                <ul class="mx-auto mt-14 flex justify-center gap-20 text-xl font-poppins">
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
            <div class="grid grid-cols-4 gap-7 mt-16">
                <div v-for="p in productoe" class="mb-16">
                    <Category :product="p" />
                </div>
            </div>
        </div>
        <div class="px-36 mt-40 h-auto">
            <div class="bg-emerald-100 rounded-sm">
                <Exclusive :product="product14" />
            </div>
        </div>
        <div class="mt-44 px-36">
            <div>
                <h2 class="font-robotoslab text-center mb-12 text-4xl">You should buy!</h2>
                <p class="font-poppins text-xl text-center">Items that should be in your shopping cart</p>
            </div>
            <div class="grid grid-cols-3 gap-9 mt-16">
                <div v-for="p in productoj">
                    <ShouldBuy :product="p" />
                </div>
            </div>
        </div>
        <div class="mt-52 px-36">
            <div>
                <h2 class="font-robotoslab text-center mb-24 text-4xl">Feedback Corner</h2>
            </div>
            <div class="grid grid-cols-3 gap-5 mx-auto">
                <div class="border-black border p-4">
                    <Icon class="mb-5" name="uil:feedback" />
                    <h1 class="font-robotoslab font-semibold text-xl mb-6">Adam Smit</h1>
                    <h2 class="font-poppins text-sm">The customer experience was exceptional from start to finish. The
                        website is user-friendly, the
                        checkout process was smooth, and the clothes I ordered fit perfectly. I'm beyond satisfied!</h2>
                </div>
                <div class="border-black border p-4">
                    <Icon class="mb-5" name="uil:feedback" />
                    <h1 class="font-robotoslab font-semibold text-xl mb-6">Lyly Anna</h1>
                    <h2 class="font-poppins text-sm">I absolutely love the quality and style of the clothing I purchased
                        from this website. customer
                        service was outstanding, and I received my order quickly. Highly recommended!</h2>
                </div>
                <div class="border-black border p-4">
                    <Icon class="mb-5" name="uil:feedback" />
                    <h1 class="font-robotoslab font-semibold text-xl">Hor Walk</h1>
                    <h2 class="font-poppins text-sm">I had a great experience shopping on this website. The clothes I bought
                        are fashionable and
                        comfortable. Highly satisfied!</h2>
                </div>
            </div>
            <div class="mt-28">
                <div class="flex justify-center gap-7">
                    <Icon class="border text-4xl" name="quill:inline-left" />
                    <Icon class="border text-4xl" name="quill:inline-right" />
                </div>
            </div>
        </div>
        <div class="bg-green-800">
            <div class="px-36 mb-36 grid grid-cols-4 h-auto max-w-full text-white mt-40">
                <div class="mt-16">
                    <h1 class="font-serif font-normal text-4xl mb-9">NUXT</h1>
                    <h2 class="font-robotoslab text-xl mb-5">Social Media</h2>
                    <div class="flex gap-4">
                        <NuxtLink to="/">
                            <Icon class="text-3xl" name="uil:github" color="white" />
                        </NuxtLink>
                        <NuxtLink to="/">
                            <Icon class="text-3xl" name="uil:twitter" color="white" />
                        </NuxtLink>
                        <NuxtLink to="/">
                            <Icon class="text-3xl" name="uil:facebook" color="white" />
                        </NuxtLink>
                    </div>
                </div>
                <div class="mt-20">
                    <h1 class="font-robotoslab text-xl mb-5">SHOP</h1>
                    <h2 class="font-poppins text-xl mb-4">Products</h2>
                    <h2 class="font-poppins text-xl mb-4">Overview</h2>
                    <h2 class="font-poppins text-xl mb-4">Pricing</h2>
                    <h2 class="font-poppins text-xl">Releases</h2>
                </div>
                <div class="mt-20">
                    <h1 class="font-robotoslab text-xl mb-5">COMPANY</h1>
                    <h2 class="font-poppins text-xl mb-4">About Us</h2>
                    <h2 class="font-poppins text-xl mb-4">Contact</h2>
                    <h2 class="font-poppins text-xl mb-4">News</h2>
                    <h2 class="font-poppins text-xl">Support</h2>
                </div>
                <div class="mt-20">
                    <h1 class="font-robotoslab text-xl mb-8">STAY UP TO DATE</h1>
                    <h2 class="w-80 flex font-poppins"><input type="text" placeholder="Enter your email"><button
                            class="bg-cyan-100 border-2 text-black">SUBMIT</button></h2>
                </div>
            </div>
            <div class="px-36 pb-16 h-auto max-w-full text-white">
                <div class="flex justify-between">
                    <hr class="my-auto w-2/3" />
                    <p class="font-poppins text-xl">Terms</p>
                    <h2 class="font-poppins text-xl">Privacy</h2>
                    <h2 class="font-poppins text-xl">Cookies</h2>

                </div>
            </div>
        </div>
    </div>
</template>

<script setup>

const { data: product7 } = await useFetch('https://fakestoreapi.com/products/7')

const { data: product14 } = await useFetch('https://fakestoreapi.com/products/14')

const { data: products } = await useFetch(`https://fakestoreapi.com/products/category/men's clothing?limit=3`)

const { data: productoj } = await useFetch(`https://fakestoreapi.com/products/category/men's clothing?limit=3&sort=desc`)

const { data: productoe } = await useFetch('https://fakestoreapi.com/products?limit=8')

const { data: productom } = await useFetch(`https://fakestoreapi.com/products/category/men's clothing`)

const { data: productow } = await useFetch(`https://fakestoreapi.com/products/category/women's clothing`)

</script>

<style scoped></style>