<script setup lang="ts">
import { ref } from 'vue'

const count = ref(0)

const incr = () => {
  count.value++
}

const desc = () => {
  count.value--
}
</script>

<template>
  <div class="couner">
    <p>{{count}}</p>
    <button @click="incr" >incr</button>
    <button @click="desc">desc</button>
  </div>
</template>