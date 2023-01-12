<script setup>
import HelloWorld from './components/HelloWorld.vue'
import TheWelcome from './components/TheWelcome.vue'
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
}

h1,
h2 {
  flex: 1;
  text-align: center;
  font-family: Badaboom;
  /* margin-top: 5pt; */
}

h1 {
  color: var(--primary)
}

h2 {
  color: var(--accent);
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }
}
</style>
