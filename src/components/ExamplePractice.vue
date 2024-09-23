<script setup>
    import { ref } from "vue";

    const counter = ref(0);

    const increment = () => {
        counter.value++;
    };

    const decrement = () => {
        counter.value--;
    };

    const reset = () => {
        counter.value = 0;
    };

    const classCounter = () => {
        if (counter.value === 0) {
            return "zero";
        }
        return counter.value > 0 ? "positive" : "negative";
    };
</script>

<template>
    <h2 :class="classCounter()">
        {{ counter }}
    </h2>

    <button @click="increment">Incremet</button>
    <button @click="decrement">Decrement</button>
    <button @click="reset">Reset</button>
</template>

<style>
.negative {
    color: red;
}

.positive {
    color: green;
}
</style>
