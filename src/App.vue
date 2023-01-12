<script setup>
import BingoCard from './components/BingoCard.vue';
import Menu from './components/Menu.vue';
</script>

<template>
  <header>
    <h1>Drag Race Bingo</h1>
    <h2>Season 15 Episode 2</h2>
  </header>
  <main>
    <BingoCard></BingoCard>
    <!-- <Menu></Menu> -->
  </main>
</template>

<style scoped>

header {
  line-height: 1.5;
  display: flex;
  flex-direction: column;
  padding:10pt;
  place-items: center;
  max-height: 25vh;
}

h1,
h2 {
  flex: 1;
  font-family: "Badaboom";
}

h1 {
  color: var(--primary);
  font-size:50pt;
}

h2 {
  color: var(--accent);
  font-size:30pt;
}

main {
  display: flex;
  place-content: center;
  width:100%;
}
</style>
