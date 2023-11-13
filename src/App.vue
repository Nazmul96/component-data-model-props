<script setup>
   import Button from './components/Button.vue'

 </script>

<template>
      <div class="container mx-auto">
        <div class="flex items-center mt-5">
          <img class="logo" src="./assets/logo.svg" alt="Vue logo" />
          <h1 class="text-2xl">Component Slot</h1>
        </div>

        <div class="mt-10">
             <Button>
                <b>Add Category</b>
              </Button>
        </div>


      </div>
</template>

<style scoped>

</style>
