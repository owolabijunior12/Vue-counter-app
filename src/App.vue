<script setup>
  import { ref } from "vue";  
  const count = ref(0)
  
</script>

<template>
  <div class="bg-black h-screen flex gap-4 flex-col items-center justify-center text-white">
    <h1  class="text-8xl font-bold font-mono">Hello World</h1>
      <h1  class="text-8xl  m-5 font-bold font-mono">{{ count }}</h1>
      <div  class="flex gap-4">
        <button   class="px-4 py-2 rounded-lg border border-green-500 hover:bg-green-600 focus:outline-none transition" @click='count++' type="button">increase</button>
         <button class="px-4 py-2 rounded-lg border border-red-500 hover:bg-red-600 focus:outline-none transition disabled:cursor-not-allowed" @click="count--" type="button">decrease</button>
      </div>

  </div>
  
</template>


