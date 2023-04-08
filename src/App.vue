<script setup lang="ts">

import Container from './components/container/Container.vue'
import Header from './components/header/Header.vue'
import SaleSection from './components/sections/sale-section/index.vue'
import TopProjectsSection from './components/sections/top-projects/index.vue'

</script>

<template>
  <Header />
  <Container>

    <SaleSection />
    <TopProjectsSection />

  </Container>
</template>