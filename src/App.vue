<script setup lang="ts">

import Container from './components/container/Container.vue'
import Header from './components/header/Header.vue'
import SaleSection from './components/sections/sale-section/index.vue'
import TopProjectsSection from './components/sections/top-projects/index.vue'
import LocationSection from './components/sections/location/index.vue'
import DetailsSection from './components/sections/details/index.vue'
import OptionsSection from './components/sections/options/index.vue'
import Footer from './components/sections/footer/index.vue'


</script>

<template>
  <Header />
  <Container>
    <SaleSection />
    <TopProjectsSection />
    <LocationSection />
    <DetailsSection />
    <OptionsSection />
  </Container>
  <Footer />
</template>