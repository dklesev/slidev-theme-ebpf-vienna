<template>
    <footer 
        v-if="$nav.currentLayout !== ('cover' && 'lead' && 'empty')" 
        class="footer footer-left">
        {{ $slidev.configs.date }}
    </footer>
    <footer 
        v-if="$nav.currentLayout !== ('cover' && 'lead' && 'empty')" 
        class="footer footer-center">
        eBPF Vienna
    </footer>
    <footer 
        v-if="$nav.currentLayout !== ('cover' && 'lead' && 'empty')" 
        class="footer footer-right">
        {{ $nav.currentPage }}
    </footer>
</template>