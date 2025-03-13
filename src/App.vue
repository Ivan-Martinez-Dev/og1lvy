<template>
  <HeroSection />
  <CounterSection />
  <CourseSection />
  <div class="container-hidden">
    <AboutSection />
    <WhySection />
  </div>

  <VideoSection />
  <UsersSection />
  <FormSection />
  <FooterSection />
</template>

<script>
import HeroSection from './components/HeroSection.vue';
import CounterSection from './components/CounterSection.vue';
import FormSection from './components/FormSection.vue';
import FooterSection from './components/layouts/FooterSection.vue';
import UsersSection from './components/UsersSection.vue';
import VideoSection from './components/VideoSection.vue';
import WhySection from './components/WhySection.vue';
import AboutSection from './components/AboutSection.vue';
import CourseSection from './components/CourseSection.vue';

export default {
  name: 'App',
  components: {
    HeroSection,
    CounterSection,
    CourseSection,
    AboutSection,
    WhySection,
    VideoSection,
    UsersSection,
    FormSection,

    FooterSection
  }
}
</script>

<style lang="scss">
@use '@/assets/styles/base/reset.scss';

.container-hidden {
  overflow: hidden;
}
</style>
