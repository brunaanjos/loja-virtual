<script setup>
import LargeAside from '@/components/teamplates/large/LargeAside.vue';
import LargeFooter from '@/components/teamplates/large/LargeFooter.vue';
import LargeHeader from '@/components/teamplates/large/LargeHeader.vue';
</script>

<template>
    <div id="large-layout">
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
    </div>
</template>
<style scoped>
#large-layout {
    display: grid;
  grid-template-columns: 1fr 5fr;
  grid-template-rows: auto 1fr auto;
  grid-template-areas:
    'aside header'
    'aside main'
    'aside footer';
  min-height: 100vh;
}

header {
  display: flex;
  widows: 100vw;
  justify-content: flex-end;
  padding: 1.5rem;
  grid-area: header;
}

aside {
  border-right: #eeeeee 1px solid;
  box-shadow: 0 0 10px 0 #a5a5a5;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  padding-top: 1.5rem;
  padding-bottom: 1.5rem;
  grid-area: aside;
}

main {
  min-height: 80%;
  padding: 2rem;
  grid-area: main;
}

footer {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 3rem;
  background-color: #e0e0e0;
  grid-area: footer;
}
</style>
