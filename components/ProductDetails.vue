<template>
     <div class="">
          <div class="grid grid-cols-2 gap-10">
               <div class="p-7">
                    <img :src="product.image" alt="product img" class="mx-auto my-7" />
               </div>
               <div class="py-7">
                    <h2 class="text-4xl my-7">{{ product.title }}</h2>
                    <p class="text-xl my-7">Price - ${{ product.price }}</p>
                    <h2 class="font-bold border-b-2 mb-4 pb-4">Product description:</h2>
                    <p class="mb-7">{{ product.description }}</p>
                    <button class="btn flex">
                        <i class="material-icons mr-2">add_shopping_cart</i>
                        <span>Add to cart</span>
                    </button>
               </div>
          </div>
          <div class=""></div>
     </div>
</template>

<script setup lang="ts">
const { product } = defineProps(["product"]);
</script>

<style scoped>
img {
     max-width: 400px;
}
</style>
