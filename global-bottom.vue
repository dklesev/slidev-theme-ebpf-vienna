<template>
    <footer 
        v-if="!['cover', 'lead', 'empty'].includes($nav.currentLayout)" 
        class="footer footer-left">
        {{ $slidev.configs.date }}
    </footer>
    <footer 
        v-if="!['cover', 'lead', 'empty'].includes($nav.currentLayout)" 
        class="footer footer-center">
        eBPF Vienna
    </footer>
    <footer 
        v-if="!['cover', 'lead', 'empty'].includes($nav.currentLayout)" 
        class="footer footer-right">
        {{ $nav.currentPage }}
    </footer>
</template>