<script setup>
import Topline from './components/Topline.vue'
import SiteHeader from './components/SiteHeader.vue'
import HeroSection from './components/HeroSection.vue'
import TickerBand from './components/TickerBand.vue'
import MenuSection from './components/MenuSection.vue'
import StorySection from './components/StorySection.vue'
import VisitSection from './components/VisitSection.vue'
import SiteFooter from './components/SiteFooter.vue'
import ReservationToast from './components/ReservationToast.vue'
</script>

<template>
  <Topline />
  <SiteHeader />
  <main>
    <HeroSection />
    <TickerBand />
    <MenuSection />
    <StorySection />
    <VisitSection />
  </main>
  <SiteFooter />
  <ReservationToast />
</template>
