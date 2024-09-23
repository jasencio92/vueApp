<template>
   <div class="post-card">
      <h3> Título </h3>
      <p> The headache wouldn't go away. She's taken medicine but even that didn't help. The monstrous throbbing in her head continued. She had this happen to her only once before in her life and she realized that only one thing could be happening. </p>
      <PostButton/>
   </div>
</template>

<script setup>
   import PostButton from './PostButton.vue';
</script>

<style scoped>
   .post-card {
      border-radius: 15px;
      padding: 10px;
      margin: 5px;
      border: 1px solid #ccc;
   }
</style>