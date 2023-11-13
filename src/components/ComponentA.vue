<script setup>
    import ComponentB from './ComponentB.vue'
    import {person} from '../store/data.js';

</script>
<template>
    <h2>Component A</h2>
    <h5>{{ person.name }}</h5>
    <ComponentB />
</template>
<style scoped>

</style>