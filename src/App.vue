<template>
  <div class="w-full h-full flex flex-col justify-center items-center">
    <div>
      <div class="w-full max-w-2xl p-4 rounded bg-red-400 text-white">
        <div class="border-2 rounded flex flex-col md:flex-row md:items-center md:gap-8 p-4">
          <img src="/assets/santa.svg" alt="" class="max-w-[12em]" />
          <div>
            <h1 class="font-serif text-4xl">Happy Holidays!</h1>
            <div class="mt-4 bg-white text-black p-2 rounded">TO: {{ to === '' ? 'John' : to }}</div>
            <div class="mt-2 bg-white text-black p-2 rounded">FROM: {{ from === '' ? 'Joana' : from }}</div>
          </div>
        </div>
      </div>
      <div class="mt-10 max-w-2xl">
        <div class="mb-2 flex">
          <label for="to">To：</label>
          <input type="text" id="to" class="border-2 border-gray-400 w-full ml-5" v-model="to" />
        </div>
        <div class="flex">
          <label for="from">From：</label>
          <input type="text" id="from" class="border-2 border-gray-400 w-full" v-model="from" />
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import { ref } from 'vue'

const from = ref('')
const to = ref('')
</script>
