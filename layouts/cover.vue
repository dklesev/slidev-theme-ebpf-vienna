<template>
  <div class="slidev-layout cover">
    <div class="my-auto w-full cover-content">
      <slot />
    </div>
    <img 
      src="/ebpf-logo.png" 
      class="logo-cover logo-light" 
      alt="eBPF logo"
    />
    <img 
      src="/ebpf-logo-dark.png" 
      class="logo-cover logo-dark" 
      alt="eBPF logo"
    />
    <div class="vienna-text">VIENNA</div>
  </div>
</template>


