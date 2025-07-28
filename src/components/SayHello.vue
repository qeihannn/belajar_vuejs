<script setup>
import {reactive} from "vue"

const person = reactive({
    firstName: "",
    lastName: ""

})

function sayHello(){
        person.firstName = document.getElementById("firstName").value;
        person.lastName = document.getElementById("lastName").value;
}
</script>

<template>
<div>
    <input placeholder="First Name" type="text" id="firstName"/> <br>
    <input placeholder="Last Name" type="text" id="lastName"/> <br>
    <button v-on:click="sayHello">Say Hello</button>
</div>
<h1>Hello {{person.firstName}} {{person.lastName}}</h1>
</template>

<style scoped>

</style>