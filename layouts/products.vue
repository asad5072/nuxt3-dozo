<template>
    <div class="container p-4">
        <header>
            <nav>
                <NuxtLink to="/">Logo</NuxtLink>
                
            </nav>
        </header> 
        <div>
            <slot />
        </div>
        <footer>
            <ul class='shadow-sm flex gap-4 bg-white p-4'>
                <li><NuxtLink to="/">Home</NuxtLink></li>
                <li><NuxtLink to="/about">About</NuxtLink></li>
                <li><NuxtLink to="/products">products</NuxtLink></li>
            </ul>
        </footer>
    </div>






  </template>

<style scoped>
    .router-link-active {
        color: red;
    }

</style>
  