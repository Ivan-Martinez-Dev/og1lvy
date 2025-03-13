<template>
    <div class="footer__items">
      <h3 class="footer__title">
        {{ title }}
      </h3>
      <div class="footer__links">
        <a v-for="(link, index) in links" :key="index" :href="link.href" class="footer__link">{{ link.text }}</a>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    name: 'FooterLinks',
    props: {
      title: {
        type: String,
        required: true
      },
      links: {
        type: Array,
        required: true
      }
    }
  };
  </script>
  
  <style scoped lang="scss">

  </style>
  