<template>
  <HeroSection />
  <CounterSection />
</template>

<script>
import HeroSection from './components/HeroSection.vue';
import CounterSection from './components/CounterSection.vue';
export default {
  name: 'App',
  components: {
    HeroSection,
    CounterSection
  }
}
</script>

<style lang="scss">
@use '@/assets/styles/base/reset.scss';
</style>
