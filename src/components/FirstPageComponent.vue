<script setup lang="ts">
    // defineProps(['title', 'likes'])

    // defineProps({
    //     title: String,
    //     likes: Number
    // })

    import { ref, computed } from "vue"
    const props = defineProps<{
        title?: string,
        likes?: number,
        employeeName: string,
        age: number,
        gender: string,
        sAge: number
    }>()

    const EName = ref(props.employeeName)
    const EAge = ref(props.age)

</script>

<template>
    <h1>First Page Component</h1>
    <!-- <div>Local EName is : {{EName}}</div> -->
    <div>Local EAge is : {{EAge}}</div>
    <div>sAge is : {{sAge}}</div>
    <div>title is : {{title}}</div>
    <div>likes is : {{likes}}</div>
    <div>employeeName is : {{ employeeName }}</div>
    <div>age is : {{ age }}</div>
    <div>gender is : {{ gender }}</div>
</template>