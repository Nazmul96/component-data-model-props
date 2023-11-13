<script setup>
    import {person} from '../store/data.js';
</script>
<template>
    <h2>Component B</h2>
    <h5>{{ person.name }}</h5>
    <input type="text" v-model="person.name">
</template>
<style scoped>

</style>