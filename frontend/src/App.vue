<script setup lang="ts">
</script>

<template>
<div class="container">
    <div class="quarter" style="background-color: lightblue; --wails-draggable: drag">Draggable</div>
    <div class="quarter" style="background-color: lightgreen;">Not Draggable</div>
    <div class="quarter" style="background-color: lightpink;">Not Draggable</div>
    <div class="quarter" style="background-color: lightyellow; --wails-draggable: drag">Draggable</div>
</div>
</template>

<style scoped>
    html, body {
        height: 100%;
        margin: 0;
        padding: 0;
    }

    .container {
        display: flex;
        flex-wrap: wrap;
        height: 100%;
    }

    .quarter {
        flex: 50%; /* This will cause elements to take up 50% of the container's width, causing them to wrap into 4 equal sections. */
        box-sizing: border-box; /* This makes the padding part of the element's total width and height, ensuring they don't exceed 50%. */
        padding: 20px;
    }

</style>
