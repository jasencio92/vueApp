<script setup>
const arrayFrutas = [
   {
      name: "Manzana",
      price: "$1.00",
      description: "Una manzana",
      stock: 0,
   },
   {
      name: "Pera",
      price: "$2.00",
      description: "Una pera",
      stock: 10,
   },
   {
      name: "Naranja",
      price: "$3.00",
      description: "Una naranja",
      stock: 20,
   }
];
</script>

<template>
   <ul>
      <template v-for="fruta in arrayFrutas" :key="fruta.name">
         <li v-if="fruta.stock > 0">
            {{ fruta }}
         </li>
      </template>
   </ul>
</template>

