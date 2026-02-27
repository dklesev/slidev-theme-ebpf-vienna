<template>
  <SlidevSpotlight />
  <img 
    v-if="!['cover', 'lead', 'empty', 'vhs'].includes($nav.currentLayout)" 
    src="/ebpf-icon.png" 
    class="logo logo-light" 
    alt="eBPF logo"
  />
  <img 
    v-if="!['cover', 'lead', 'empty', 'vhs'].includes($nav.currentLayout)" 
    src="/ebpf-icon-dark.png" 
    class="logo logo-dark" 
    alt="eBPF logo"
  />
</template>