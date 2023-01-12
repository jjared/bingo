<script setup>
import BingoTile from './BingoTile.vue';

const tiles = [
"Ariana Grande",
"RuPaul laughs at something that's not funny",
"RuPaul calls Michelle \"Squirrelfriend\"",
"No one goes home",
"\"But this year, there's a twist\"",
"\"I'm coming for the crown\"",
"Sasha Colby is referred to as a legend at least 3 times",
"A queen is surprised by the boy looks when everyone de-drags",
"Punny entrance line",
"Death drop and/or splits",
"One of the judges definitely did coke",
"Split premier - see you next week"
];
while (25 > tiles.length) {
  tiles.push("");
}
</script>

<template>
  <table>
  <tr v-for="i in [0,1,2,3,4]">
  <BingoTile v-for="tile in tiles.slice(5*i, 5*(i+1))" :tile=tile></BingoTile>
  </tr>
  </table>
</template>

<style scoped>
table {
  place-items: center;
  border-color: var(--dark);
  background-color: var(--secondary);
  border-width:5pt;
  border-style: hidden;
  border-radius:10pt;
  border-collapse:collapse;
  box-shadow: 0 0 0 5pt var(--primary);
  max-width:75%;
  flex:0.7;
  margin:20pt;
  font-family: "Bianca";
}

</style>
