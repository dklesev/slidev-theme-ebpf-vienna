<script setup>
import ebpfLogo from '../public/ebpf-logo.png'
import ebpfLogoDark from '../public/ebpf-logo-dark.png'
</script>

<template>
  <div class="slidev-layout cover">
    <div class="my-auto w-full cover-content">
      <slot />
    </div>
    <img
      :src="ebpfLogo"
      class="logo-cover logo-light"
      alt="eBPF logo"
    />
    <img
      :src="ebpfLogoDark"
      class="logo-cover logo-dark"
      alt="eBPF logo"
    />
    <div class="vienna-text">VIENNA</div>
  </div>
</template>


