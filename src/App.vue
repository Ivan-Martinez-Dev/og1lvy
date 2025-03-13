<template>
  <HeroSection />
  <CounterSection />
  <VideoSection />
  <UsersSection />
  <FormSection/>
  <FooterSection />
</template>

<script>
import HeroSection from './components/HeroSection.vue';
import CounterSection from './components/CounterSection.vue';
import FormSection from './components/FormSection.vue';
import FooterSection from './components/layouts/FooterSection.vue';
import UsersSection from './components/UsersSection.vue';
import VideoSection from './components/VideoSection.vue';
export default {
  name: 'App',
  components: {
    HeroSection,
    CounterSection,
    VideoSection,
    UsersSection,
    FormSection,
    
    FooterSection
  }
}
</script>

<style lang="scss">
@use '@/assets/styles/base/reset.scss';
</style>
