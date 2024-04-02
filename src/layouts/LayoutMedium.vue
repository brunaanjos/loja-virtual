<script setup>
import MediumAside from '@/components/teamplates/medium/MediumAside.vue';
import MediumFooter from '@/components/teamplates/medium/MediumFooter.vue';
import MediumHeader from '@/components/teamplates/medium/MediumHeader.vue';
</script>

<template>
    <header>
        <medium-header />
    </header>

    <aside>
        <medium-aside />
    </aside>

    <main>
        <router-view />
    </main>

    <footer>
        <medium-footer />
    </footer>

</template>