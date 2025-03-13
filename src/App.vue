<template>
  <HeroSection />
  <CounterSection />
  <FooterSection />
</template>

<script>
import HeroSection from './components/HeroSection.vue';
import CounterSection from './components/CounterSection.vue';
import FooterSection from './components/layouts/FooterSection.vue';
export default {
  name: 'App',
  components: {
    HeroSection,
    CounterSection,
    FooterSection
  }
}
</script>

<style lang="scss">
@use '@/assets/styles/base/reset.scss';
</style>
