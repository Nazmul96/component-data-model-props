<script setup>
    const props = defineProps(['fname','lname']);
    const emit = defineEmits(['update:fname','update:lname'])
</script>

<template>
       <h2>child component</h2>
       <p>
        <label>Name</label> <br />
        <input type="text" :value="fname" @input="$emit('update:fname', $event.target.value)"><br/>
        <label>Email</label> <br />
        <input type="text" :value="lname" @input="$emit('update:lname', $event.target.value)"><br/>
      </p>
</template>

<style scoped>
</style>