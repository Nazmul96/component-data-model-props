<script setup>
    const props = defineProps([
            'person'
    ])

</script>
<template>
       <h2>child component</h2>
       <p>
        <label>Name</label> <br />
        <input type="text" v-model="person.name"><br/>
        <label>Email</label> <br />
        <input type="text" v-model="person.email"><br/>
      </p>
</template>
<style scoped>

</style>