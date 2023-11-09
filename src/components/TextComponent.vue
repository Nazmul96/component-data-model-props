<script setup>
    const props = defineProps([
        'label','modelValue'
    ])
    const emit = defineEmits(['update:modelValue'])
</script>
<template>
       <h2>child component</h2>
       <p>
        <label>{{ label }}</label> <br/>
        <input type="text" :value="modelValue" @input="$emit('update:modelValue', $event.target.value)">
      </p>
</template>
<style scoped>

</style>