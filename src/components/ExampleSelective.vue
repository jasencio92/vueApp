<template>
   <h1 v-if="age >= 18"> Eres mayor de edad </h1>
   <h1 v-else> Eres menor de edad </h1>
</template>

<script setup>
   let age = 15;
</script>

<style scoped>
   h1 { color : red; }
</style>