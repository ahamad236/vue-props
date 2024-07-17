<script setup lang="ts">
    defineProps({
        // title: {
        //     type: String,
        //     required: true
        // },
        title: [String, null],
        // age: Number, 
        age: {
            type: Number,
            default: 18
        },
        isAlive: Boolean,
        salary: [String, Boolean]
    })
</script>

<template>
    <h1>Second Page Component Related to Props Validation</h1>
    <div>title is : {{title}}</div>
    <div>age is : {{age}}</div>
    <div>isAlive is : {{isAlive}}</div>
    <div>Salary is : {{ salary }}</div>
</template>