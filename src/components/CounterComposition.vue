<template>
   <h3>{{ counter }}</h3>
   <button @click="addCounter"> Incrementar Composition </button>
   <button @click="lessCounter"> Decrementar Composition </button>
</template>

<script setup>
   import { ref } from 'vue';
   let counter = ref(0);
   const addCounter = ()=>{
      counter.value++
   }
   const lessCounter = ()=>{
      counter.value--
   }
</script>