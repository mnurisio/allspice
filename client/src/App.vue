<script setup>
import Navbar from './components/Navbar.vue';
import { AppState } from './AppState.js';
import RecipeModal from './components/RecipeModal.vue';

</script>

<template>
  <header>
    <Navbar />
  </header>
  <main>
    <router-view />
  </main>

  <RecipeModal />
</template>

<style lang="scss">
@import '@/assets/scss/main.scss';
:root {
  --main-height: calc(100vh - 32px - 64px);
}

footer {
  display: grid;
  place-content: center;
  height: 32px;
}

::-webkit-scrollbar {
    width: 8px;
}


::-webkit-scrollbar-track {
    background: #f1f1f1;
    border-radius: 4px;
}


::-webkit-scrollbar-thumb {
    background: #219653;
    border-radius: 4px;
}


::-webkit-scrollbar-thumb:hover {
    background: #176d73;
}
</style>
