<script setup>
import {ref} from "vue";

const score = ref(100);
</script>

<template>
    <h1>Score App</h1>
    <div v-if="score > 90">
        <p>Yay Cool Score {{ score }}</p>
    </div>
    <div v-else-if="score > 70">
        <p>Good Score{{ score }}</p>

    </div>
    <div v-else>
        <p>Ups, bad score</p>
    </div>

</template>

<style scoped>

</style>