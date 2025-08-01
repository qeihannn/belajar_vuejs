<script setup>
const item = [{
    id: 1,
    text: "Learn Vue 3",
},{
    id: 2,
    text: "Learn Vue Router",
}, {
    id: 3,
    text: "Learn Vuex",
}];

</script>

<template>
    <h1>Todo List</h1>
    <ul>
        <li v-for="item in items">
            {{item.text }}
        </li>
    </ul>
</template>

<style scoped>

</style>