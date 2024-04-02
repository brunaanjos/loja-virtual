<script setup>
import SmallFooter from '@/components/teamplates/small/SmallFooter.vue';
import SmallHeader from '@/components/teamplates/small/SmallHeader.vue';
</script>

<template>
    <header>
        <small-header />
    </header>

    <aside>
        <small-aside />
    </aside>

    <main>
        <router-view />
    </main>

    <footer>
        <small-footer />
    </footer>

</template>