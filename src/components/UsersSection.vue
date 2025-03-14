<template>
    <section class="users">
        <div class="users__container">
            <h2 class="users__title">What</h2>
            <h2 class="users__title subtitle">users think.</h2>
        </div>
        <div class="users__swiper">
            <swiper ref="mySwiper" :slidesPerView="1" :spaceBetween="10" :loop="true" :navigation="{
                nextEl: '.users__swiper--next',
                prevEl: '.users__swiper--prev'
            }" 
            :breakpoints="{
                992: {
                    slidesPerView: 3,
                    spaceBetween: 0
                }
            }" :modules="modules">
                <!-- Cada slide -->
                <swiper-slide>
                    <div class="users__card">
                        <div class="users__profile">
                            <img src="@/assets/images/profile-1.png" alt="Imagen Estática" />
                        </div>
                        <p class="users__name">Laura smith</p>
                        <div class="users__stars">
                            <img src="@/assets/images/stars.png" alt="">
                        </div>
                        <div class="users__testimony">
                            <img src="@/assets/images/Quote-1.png" alt="" class="users__testimony--quote">
                            <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor
                                incididunt ut labore et dolore magna aliqua .</p>
                            <img src="@/assets/images/Quote-2.png" alt="" class="users__testimony--quote type-02">
                        </div>
                    </div>
                </swiper-slide>
                <swiper-slide>
                    <div class="users__card">
                        <div class="users__profile">
                            <img src="@/assets/images/profile-2.png" alt="Imagen Estática" />
                        </div>
                        <p class="users__name">Jhon smith</p>
                        <div class="users__stars">
                            <img src="@/assets/images/stars.png" alt="">
                        </div>
                        <div class="users__testimony">
                            <img src="@/assets/images/Quote-1.png" alt="" class="users__testimony--quote">
                            <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor
                                incididunt ut labore et dolore magna aliqua .</p>
                            <img src="@/assets/images/Quote-2.png" alt="" class="users__testimony--quote type-02">
                        </div>
                    </div>
                </swiper-slide>
                <swiper-slide>
                    <div class="users__card">
                        <div class="users__profile">
                            <img src="@/assets/images/profile-3.png" alt="Imagen Estática" />
                        </div>
                        <p class="users__name">Sara smith</p>
                        <div class="users__stars">
                            <img src="@/assets/images/stars.png" alt="">
                        </div>
                        <div class="users__testimony">
                            <img src="@/assets/images/Quote-1.png" alt="" class="users__testimony--quote">
                            <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor
                                incididunt ut labore et dolore magna aliqua .</p>
                            <img src="@/assets/images/Quote-2.png" alt="" class="users__testimony--quote type-02">
                        </div>
                    </div>
                </swiper-slide>
            </swiper>
            <div class="users__swiper--controls">
                <button class="btn__swiper users__swiper--prev">
                    <img src="@/assets/images/Arrow-1.png" alt="Flecha Izquierda">
                </button>
                <button class="btn__swiper users__swiper--next">
                    <img src="@/assets/images/Arrow-2.png" alt="Flecha Derecha">
                </button>
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
    name: 'UsersSection',
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
@use '@/assets/styles/components/users.scss';
@use '@/assets/styles/components/buttons.scss';
</style>