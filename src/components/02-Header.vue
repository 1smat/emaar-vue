<script setup lang="ts">


defineProps<{ msg?: string }>()


</script>

<template>
    <header class="header">
        <h1>header h1</h1>
    </header>
</template>

<style scoped lang="scss">
.header {
    h1 {
        color: red;
    }
}
</style>
