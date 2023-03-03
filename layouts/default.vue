<template>
    <div>
        <header class="shadow-sm bg-white">
            <nav class="container mx-auto p-4 flex justify-between">
                <NuxtLink to="/" class="font-bold">Logo</NuxtLink>
                <ul class="flex gap-4">
                    <li><NuxtLink to="/">Home</NuxtLink></li>
                    <li><NuxtLink to="/about">About</NuxtLink></li>
                    <li><NuxtLink to="/products" class="btn">products</NuxtLink></li>
                </ul>
            </nav>
        </header> 
    </div>

    <div  class="container mx-auto p-4">
        <slot />
    </div>

    
  </template>

<style scoped>
    .router-link-active {
        color: red;
    }

</style>
  