<template>
  <SlidevSpotlight />
  <img 
    v-if="!['cover', 'lead', 'empty'].includes($nav.currentLayout)" 
    src="https://ebpf.foundation/wp-content/uploads/sites/9/2023/03/ebpf-icon-292x300.png" 
    class="logo" 
    alt="eBPF logo"
  />
</template>
