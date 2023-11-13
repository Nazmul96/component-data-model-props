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
                <template #licon>
                  <svg height="20" viewBox="0 0 128 128" width="20" xmlns="http://www.w3.org/2000/svg" id="fi_4208490">
                  <g>
                    <circle cx="64.001" cy="63.999" fill="#f24646" r="45"></circle>
                    <path d="m54.44 84.253 31.788-18.353a2.195 2.195 0 0 0 0-3.8l-31.788-18.355a2.2 2.2 0 0 0 -3.293 1.9v36.707a2.2 2.2 0 0 0 3.293 1.901z" fill="#fffcee"></path>
                  </g>
                  </svg>
                </template>  
                <template #default><b>Add Category</b></template>
                <template #ricon>
                <svg height="20" viewBox="0 0 128 128" width="20" xmlns="http://www.w3.org/2000/svg" id="fi_4208490">
                <g>
                  <circle cx="64.001" cy="63.999" fill="#f24646" r="45"></circle>
                  <path d="m54.44 84.253 31.788-18.353a2.195 2.195 0 0 0 0-3.8l-31.788-18.355a2.2 2.2 0 0 0 -3.293 1.9v36.707a2.2 2.2 0 0 0 3.293 1.901z" fill="#fffcee"></path>
                </g>
                </svg>
              </template> 
              </Button>
        </div>


      </div>
</template>

<style scoped>

</style>
