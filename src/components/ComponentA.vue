<script setup>
    import ComponentB from './ComponentB.vue'
    import {inject} from 'vue';
    // const props = defineProps(['person']);
    const person = inject('person');
</script>
<template>
    <h2>Component A</h2>
    <h5>{{ person.name }}</h5>
    <ComponentB />
</template>
<style scoped>

</style>