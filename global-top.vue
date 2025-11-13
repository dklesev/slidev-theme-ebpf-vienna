<script setup lang="ts">
import { computed } from 'vue'
import { useNav } from '@slidev/client'

const nav = useNav()

const showLogo = computed(() => 
  !['cover', 'lead', 'empty'].includes(nav.currentLayout.value)
)
</script>

<template>
  <SlidevSpotlight />
  <img 
    v-if="showLogo" 
    src="https://ebpf.foundation/wp-content/uploads/sites/9/2023/03/ebpf-icon-292x300.png" 
    class="logo" 
    alt="eBPF logo"
  />
</template>
