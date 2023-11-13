<script setup>
    // const props = defineProps(['person'])
    import {inject} from 'vue';
    const person = inject('person');
</script>
<template>
    <h2>Component B</h2>
    <h5>{{ person.name }}</h5>
</template>
<style scoped>

</style>