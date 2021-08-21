<template>
  <h1>{{ msg }}</h1>

  <button class="bg-blue-500 hover:bg-blue-800 text-white" type="button" @click="state.count++">
    count is: {{ state.count }}
  </button>
</template>

<script setup>
import { defineProps, reactive } from 'vue'

defineProps({
  msg: String
})

const state = reactive({ count: 0 })
</script>

<style scoped>
a {
  color: #42b983;
}
</style>
