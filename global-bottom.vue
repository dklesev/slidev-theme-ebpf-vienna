<template>
    <footer 
        v-if="$nav.currentLayout !== ('cover' && 'lead')" 
        class="footer footer-left">
        {{ $slidev.configs.date }}
    </footer>
    <footer 
        v-if="$nav.currentLayout !== ('cover' && 'lead')" 
        class="footer footer-center">
        eBPF Vienna
    </footer>
    <footer 
        v-if="$nav.currentLayout !== ('cover' && 'lead')" 
        class="footer footer-right">
        {{ $nav.currentPage }}
    </footer>
</template>