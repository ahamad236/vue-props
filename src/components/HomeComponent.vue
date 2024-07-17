<script setup lang="ts">
    import FirstPage from "./FirstPageComponent.vue"
    import { ref } from "vue"

    // Related to FirstPage
    const Employee = ref({
        employeeName: "Ahamad",
        age: 27,
        gender: "Male"
    })
    const sAge = ref(18)
    // Related to FirstPage Upto above


    // Related to SecondPage
    import SecondPage from "./SecondPageComponent.vue"
    // Related to SecondPage Upto above

</script>

<template>
    <h1>Home Component</h1>

    <!-- Related to FirstPage -->
    <button @click="++Employee.age">EAge is {{ Employee.age }}</button>
    <FirstPage title="Hello World" :likes="5" v-bind="Employee" :sAge="sAge"></FirstPage>
    <!-- Related to FirstPage Upto above -->


    <!-- Related to SecondPage -->
    <SecondPage :age=27 :isAlive="false" salary></SecondPage>
    <!-- Related to SecondPage Upto above -->


</template>