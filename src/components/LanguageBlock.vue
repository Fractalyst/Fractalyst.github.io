<script setup lang="ts">
</script>

<template>
    <div class="overview-item">
        <div class="icons">
            <slot name="icon"></slot>
        </div>
        <slot></slot>
    </div>
</template>


<style scoped>
.icons {
    width: min-content;
    font-size: 50px;
}

.overview-item {
    display: flex;
    border-width: 2px;
    border-color: white;
    border-radius: 16px;
    border-style: solid;
    padding: 16px;
    margin: 16px;
}
</style>