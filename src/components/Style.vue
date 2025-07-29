<script setup>

import {ref} from "vue"

const red = ref(false)
const bold = ref(false)

function toggleRed() {
red.value = !red.value
}

function toggleBold() {
    bold.value = !bold.value
}

</script>

<template>
<h1 :class="{red: red, bold: bold}">Style</h1>
<h1 :class="['red', 'bold']">style</h1>
<button v-on:click="toggleRed">Red</button>
<button v-on:click="toggleBold">Bold</button>
</template>

<style scoped>
.red {
    color: red;
}

.bold {
    text-transform: uppercase;
    font-weight: bold;
}
</style>