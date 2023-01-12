<script setup>
import BingoCard from './components/BingoCard.vue';
</script>

<template>
  <div id="theme" class="theme-dark">
  <header>
  <h1>Drag Race Bingo</h1>
  <h2>Season 15 Episode 2</h2>
  </header>
  <main>
  <BingoCard></BingoCard>
  <Menu></Menu>
  </main>
</div>
</template>

<style scoped>
#theme {
  background-color: var(--background);
  display: block;
  height: 100vh;
  width: 100vw;
}

header {
  line-height: 1.5;
  display: flex;
  flex-direction: column;
  padding:10pt;
  place-items: center;
}

h1,
h2 {
  flex: 1;
  font-family: Badaboom;
}

h1 {
  color: var(--primary)
}

h2 {
  color: var(--accent);
}

main {
  display: flex;
  place-content: center;
  width:100%;
}
</style>
