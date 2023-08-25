<script setup>
import { ref } from 'vue'

const count = ref(0)
</script>
<template>
  <div class="bg-slate-200 w-screen h-screen">
    <div class="flex items-center justify-center h-full">
      <div class="text-center">
        <h4 class="text-2xl">
          The current count is <span>{{ count }}</span>
        </h4>
        <h1 class="text-7xl">{{ count }}</h1>
        <div class="mt-4">
          <button class="border py-1 px-8 rounded bg-emerald-300" @click="count--">-</button>
          <button class="border py-1 px-8 rounded bg-emerald-300" @click="count++">+</button>
        </div>
      </div>
    </div>
  </div>
</template>