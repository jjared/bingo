<script>
import VueResizeText from 'vue3-resize-text';

export default {
    props: {
        tile: String
    },
    directives: {
        ResizeText: VueResizeText.ResizeText
    }
}
</script>

<template>
    <td>
        <!-- <div class="tilewrapper"> -->
            <div class="tile"><span v-resize-text="{ratio:1.3, minFontSize: '30px', maxFontSize: '100px', delay: 200}">{{ tile }}</span></div>
        <!-- </div> -->
    </td>
</template>

<style scoped>
.tilewrapper {
    padding-bottom:100%;
    height:0;
    width:100%;
    place-items:center;
}
.tile {
    display: table;
    height:100%;
    width:100%;
    aspect-ratio: 1/1;
}

span {
    display: table-cell;
    vertical-align: middle;
    text-align: center;
    padding: 2pt;
    height:100%;
    /* font-size: 5px; */
}

td {
    border-color: var(--primary);
    border-style: solid;
    border-width: 2px;
    width:20%;
}

</style>