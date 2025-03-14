<template>
  <section class="hero">
    <div class="hero__container">
      <div class="hero__container--type-11">
        <div class="hero__container--type-02">
          <div class="hero__container--type-04">
            <p class="hero__text type-01">
              ui<span>.</span>
            </p>
            <div class="hero__container--type-05">
              <p class="hero__text type-02">BEGINNER<span>′s</span></p>
              <div class="hero__container--type-06">
                <div class="hero__square"></div>
                <p class="hero__text type-03">become a <br>
                  pro-designer</p>
              </div>

              <button class="btn__swiper hero__swiper--prev">
                <img src="@/assets/images/Arrow-1.png" alt="Flecha Izquierda">
              </button>
            </div>
          </div>
        </div>
        <div class="hero__container--type-08">
          <img src="@/assets/images/circle-hero.png" alt="circulo fondo slider">
        </div>
        <div class="hero__container--type-03">
          <div class="hero__container--type-07">
            <p class="hero__text type-04">Edition <br>
              <span>2022</span>
            </p>
          </div>
          <div class="hero__container--type-09">
            <p class="hero__text title">Start guide for beginner
              designers</p>
            <p class="hero__text description">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod
              tempor
              incididunt ut labore .</p>
            <div class="hero__container--type-10">
              <button class="btn__primary hero">let´s start</button>
              <button class="btn__tertiary hero">read more</button>
            </div>
          </div>
          <button class="btn__swiper hero__swiper--next">
            <img src="@/assets/images/Arrow-2.png" alt="Flecha Derecha">
          </button>
        </div>
      </div>
    </div>
    <div class="hero__container--type-12">
      <swiper ref="mySwiper" :slidesPerView="1" :spaceBetween="10" :loop="true" :speed="1000" :navigation="{
        nextEl: '.hero__swiper--next',
        prevEl: '.hero__swiper--prev'
      }" :modules="modules">
        <!-- Cada slide -->
        <swiper-slide>
          <div class="hero__person">
            <img src="@/assets/images/hombre-hero.png" alt="Hombre ubicado en el hero de la pagina">
          </div>
        </swiper-slide>
        <swiper-slide>
          <div class="hero__person">
            <img src="@/assets/images/hombre-hero.png" alt="Hombre ubicado en el hero de la pagina">
          </div>
        </swiper-slide>
        <swiper-slide>
          <div class="hero__person">
            <img src="@/assets/images/hombre-hero.png" alt="Hombre ubicado en el hero de la pagina">
          </div>
        </swiper-slide>
      </swiper>
    </div>
    <div class="hero__container--type-13">
        <p class="hero__text title">Start guide for beginner
          designers</p>
        <p class="hero__text description">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod
          tempor
          incididunt ut labore .</p>
        <div class="hero__container--type-10">
          <button class="btn__primary hero">let´s start</button>
          <button class="btn__tertiary hero">read more</button>
        </div>
      </div>
  </section>
</template>

<script>
// Importar Swiper y sus módulos
import { Navigation } from 'swiper/modules';
// Import Swiper Vue.js components
import { Swiper, SwiperSlide } from 'swiper/vue';

// Import Swiper styles
import 'swiper/css';
import 'swiper/css/navigation';

export default {
  name: 'HeroSection',
  components: {
    Swiper,
    SwiperSlide,
  },
  setup() {
    const onSwiper = (swiper) => {
      console.log(swiper);
    };
    const onSlideChange = () => {
      console.log('slide change');
    };

    return {
      onSwiper,
      onSlideChange,
      modules: [Navigation],
    };
  },
};
</script>
<style lang="scss">
@use '@/assets/styles/components/hero.scss';
@use '@/assets/styles/components/buttons.scss';
</style>