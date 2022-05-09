<template>
  <div class="h-full bg-gradient-to-b from-indigo-200 to-indigo-100">
    Content
  </div>
</template>

<script lang="ts">
import { defineComponent, toRef, ref } from 'vue'
import { globalState } from '../store'

export default defineComponent({

  setup() {
    return {
      count: toRef(globalState, 'count'),
      name: ref(''),
    }
  },
})
</script>

<style>

</style>
