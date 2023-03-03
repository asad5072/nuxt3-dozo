<template>
    <div>

        <h2>product details for {{ id }}</h2>
    
        <p>Name: {{product.title}}</p>
        <p>price: {{product.price}}</p>
        <p>id: {{product.id}}</p>
    </div>
</template>

<script setup>
    const { id } = useRoute().params
    const uri = 'https://fakestoreapi.com/products' + id
    
    //fetch the product
    const {data: product} =await useFetch(uri, {key: id})
</script>