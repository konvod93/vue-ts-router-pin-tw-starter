<script setup lang="ts">
import { ref } from 'vue'

defineProps<{ msg: string }>()

const count = ref(0)
</script>

<template>
  <h1 class="text-4xl font-bold text-green-700">{{ msg }} </h1>

  <div class="flex flex-col items-center">
    <button type="button" @click="count++" class="bg-blue-300 border-1 border-blue-700 shadow-gray-900 shadow-2xl rounded-md m-16 pr-2 pl-2">count is {{ count }}</button>
    <p class="m-4">
      Edit
      <code>components/HelloWorld.vue</code> to test HMR
    </p>
  </div>

  <p class="m-2 font-bold text-2xl text-blue-600">
    This is  Vue + Vite starter template with TypeScript, Vue Router, Pinia and fixed bugs of initial setup.
  </p>
  <p>
    Learn more about IDE Support for Vue in the
    <a
      href="https://vuejs.org/guide/scaling-up/tooling.html#ide-support"
      target="_blank"
      class="font-bold text-blue-300"
      >Vue Docs Scaling up Guide</a
    >.
  </p>
  <p class="read-the-docs">Click on the Vite and Vue logos to learn more</p>
</template>

<style scoped>
/* Add your custom styles here */
</style>
