<template>
   <h3> {{ counter }} </h3>
   <button @click="addCouter">Incrementar Option</button>
</template>

<script>
   // OptionAPi
   import { defineComponent } from 'vue';
   export default defineComponent({
      name: 'CounterOption',
      data(){
         let counter = 0;
         return { counter }
      },
      methods: {
         addCouter(){
            this.counter++;
         }
      }
   })
</script>

<style> </style>