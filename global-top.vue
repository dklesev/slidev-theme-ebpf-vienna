<script setup>
import ebpfIcon from './public/ebpf-icon.png'
import ebpfIconDark from './public/ebpf-icon-dark.png'
</script>

<template>
  <SlidevSpotlight />
  <img
    v-if="!['cover', 'lead', 'empty', 'vhs'].includes($nav.currentLayout)"
    :src="ebpfIcon"
    class="logo logo-light"
    alt="eBPF logo"
  />
  <img
    v-if="!['cover', 'lead', 'empty', 'vhs'].includes($nav.currentLayout)"
    :src="ebpfIconDark"
    class="logo logo-dark"
    alt="eBPF logo"
  />
</template>