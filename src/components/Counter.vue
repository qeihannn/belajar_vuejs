<script setup>
import {ref} from "vue";

console.info(`Load component`);
let counter = ref({
    count: 0,
    name: "qeihannn"
});

function increment() {
    console.info(`Increment counter : ${counter.value.count}`);
    counter.value = {
        name: counter.value.name,
        count: counter.value.count + 1
     }
}
</script>

<template>
<div>
    <h1 id="count">Counter {{ counter.name }} :{{counter.count}}</h1>
    <button v-on:click="increment">Increment</button>
</div>
</template>

<style scoped>

</style>