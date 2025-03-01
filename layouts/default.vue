<template>
    <div class="slidev-layout default">
        <slot />
    </div>
</template>
  

<script setup>
  import { onMounted } from 'vue'

  // This code will run once when the layout is mounted,
  // applying the transformation to all h1 elements on every slide.
  onMounted(() => {
  // Use querySelectorAll in case there are multiple h1 elements.
  const headers = document.querySelectorAll('h1')
  headers.forEach(h1 => {
      const text = h1.textContent
      const pipeIndex = text.indexOf('|')
      if (pipeIndex !== -1) {
      const beforePipe = text.substring(0, pipeIndex)
      const afterPipe = text.substring(pipeIndex)
      h1.innerHTML = beforePipe + '<span class="transparent">' + afterPipe + '</span>'
      }
  })
  })
</script>