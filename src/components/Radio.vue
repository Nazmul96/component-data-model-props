<script setup>
    import {computed} from 'vue'
    const props = defineProps(['label','value','modelValue']);
    const emit  = defineEmits(['update:modelValue'])
    const radioValue = computed({
                            get: () => props.modelValue,
                            set: (value) => emit('update:modelValue', value)
                      })
</script>

<template>
       <p>
        <label>{{label}}</label> <br />
        <input class="ml-2" type="radio" :value="value" v-model="radioValue">
      </p>
</template>

<style scoped>
</style>