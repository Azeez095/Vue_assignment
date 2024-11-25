<script setup>
    import data from "../data.json"
    import { ref } from "vue"

    const dataStore = ref(data)
</script>

<template>
    console.log(dataStore)
</template>