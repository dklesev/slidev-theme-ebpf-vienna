<script setup lang="ts">
import { computed } from 'vue'
import { useNav } from '@slidev/client'

const nav = useNav()

const showFooter = computed(() => 
  !['cover', 'lead', 'empty'].includes(nav.currentLayout.value)
)
</script>

<template>
  <template v-if="showFooter">
    <footer class="footer footer-left">
      {{ $slidev.configs.date }}
    </footer>
    <footer class="footer footer-center">
      eBPF Vienna
    </footer>
    <footer class="footer footer-right">
      {{ nav.currentPage }}
    </footer>
  </template>
</template>
