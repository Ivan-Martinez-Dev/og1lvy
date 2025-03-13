<template>
  <HeroSection />
  <CounterSection />
  <FormSection/>
  <FooterSection />
</template>

<script>
import HeroSection from './components/HeroSection.vue';
import CounterSection from './components/CounterSection.vue';
import FormSection from './components/FormSection.vue';
import FooterSection from './components/layouts/FooterSection.vue';
export default {
  name: 'App',
  components: {
    HeroSection,
    CounterSection,
    FormSection,
    FooterSection
  }
}
</script>

<style lang="scss">
@use '@/assets/styles/base/reset.scss';
</style>
