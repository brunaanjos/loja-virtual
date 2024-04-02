<script setup>
import LargeAside from '@/components/teamplates/large/LargeAside.vue';
import LargeFooter from '@/components/teamplates/large/LargeFooter.vue';
import LargeHeader from '@/components/teamplates/large/LargeHeader.vue';
</script>

<template>
    <header>
        <large-header />
    </header>

    <aside>
        <large-aside />
    </aside>

    <main>
        <router-view />
    </main>

    <footer>
        <large-footer />
    </footer>

</template>