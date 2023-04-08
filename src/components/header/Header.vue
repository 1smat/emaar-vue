<script setup lang="ts">
import Card from './Card.vue';


defineProps<{ msg?: string }>()


</script>

<template>
    <header class="header">
        <card />
    </header>
</template>

<style scoped lang="scss">
.header {
    position: relative;
    height: 100vh;
    background-image: url('../../assets/img/header-bg.svg');
    background-size: cover;
    background-repeat: no-repeat;

    h1 {
        color: red;
    }
}
</style>
