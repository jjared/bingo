<script>
export default {
    props: {
        tile: String
    }
}
</script>

<template>
    <td>{{ tile }}</td>
</template>

<style scoped>
td {
    border-color: var(--secondary);
    padding: 10pt;
    place-content: center;
}
</style>