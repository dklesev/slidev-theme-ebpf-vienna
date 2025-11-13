<script setup lang="ts">
import { onMounted } from 'vue'

// Transform h1 elements with pipe separator for styling
onMounted(() => {
  const headers = document.querySelectorAll('.slidev-layout.default h1')
  headers.forEach((h1) => {
    const text = h1.textContent || ''
    const pipeIndex = text.indexOf('|')
    
    if (pipeIndex !== -1) {
      const beforePipe = text.substring(0, pipeIndex)
      const afterPipe = text.substring(pipeIndex)
      h1.innerHTML = `${beforePipe}<span class="transparent">${afterPipe}</span>`
    }
  })
})
</script>

<template>
  <div class="slidev-layout default">
    <slot />
  </div>
</template>
