<script setup>
import ebpfIconDark from '../public/ebpf-icon-dark.png'
</script>

<template>
  <div class="slidev-layout vhs">
    <img
      :src="ebpfIconDark"
      class="logo-vhs"
      alt="eBPF logo"
    />
    <slot />
  </div>
</template>
