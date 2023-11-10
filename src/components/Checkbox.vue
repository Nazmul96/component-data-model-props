<script setup>
    import {ref} from 'vue'
    const props = defineProps(['label','modelValue']);
    const emit  = defineEmits(['update:modelValue'])
</script>

<template>
       <h2>child component</h2>
       <p>
        <label>{{label}}</label> <br />
        <input type="checkbox" :checked="modelValue"  @change="$emit('update:modelValue',$event.target.checked)">
      </p>
</template>

<style scoped>
</style>