<script setup>
    import {ref} from 'vue'
    const props = defineProps(['modelValue']);
    const new_name = props.modelValue.split(' ');
    const fname = ref(new_name[0]);
    const lname = ref(new_name[1]);
    const emit = defineEmits(['update:modelValue']);
    function updatename(){
        emit('update:modelValue',`${fname.value} ${lname.value}`)
    }
</script>

<template>
       <h2>child component</h2>
       <p>
        <label>Name</label> <br />
        <input type="text" v-model="fname" @input="updatename()"><br/>
        <label>Email</label> <br />
        <input type="text" v-model="lname" @input="updatename()"><br/>
      </p>
</template>

<style scoped>
</style>