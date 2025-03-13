<template>
    <section class="course">
        <div class="course__container">
            <div class="course__container--type-02">
                <h2 class="course__text">Find <span>your course.</span></h2>
                <div class="course__container--type-03">
                    <div class="course__square"></div>
                    <div class="course__container--type-04">
                        <p class="course__text type-02">Edition</p>
                        <p class="course__text type-03">2022</p>
                    </div>
                </div>
            </div>

        </div>
        <div class="course__swiper">
            <swiper ref="mySwiper" :slidesPerView="1" :spaceBetween="10" :loop="true" :navigation="{
                nextEl: '.course__swiper--next',
                prevEl: '.course__swiper--prev'
            }" :breakpoints="{
                992: {
                    slidesPerView: 4,
                    spaceBetween: 0
                }
            }" :modules="modules">
                <!-- Cada slide -->
                <swiper-slide>
                    <div class="course__card">
                        <div class="course__card--number">.01</div>
                        <p class="course__card--title">Course <span>01</span></p>
                        <div class="course__card--decorator"></div>
                        <p class="course__card--description">Lorem ipsum dolor sit amet, consectetur adipiscing
                            elit, sed
                            do eiusmod tempor incididunt ut labore et.</p>
                        <a href="" class="btn__primary card">Read More</a>
                    </div>
                </swiper-slide>
                <swiper-slide>
                    <div class="course__card">
                        <div class="course__card--number">.02</div>
                        <p class="course__card--title">Course <span>02</span></p>
                        <div class="course__card--decorator"></div>
                        <p class="course__card--description">Lorem ipsum dolor sit amet, consectetur adipiscing
                            elit, sed
                            do eiusmod tempor incididunt ut labore et.</p>
                        <a href="" class="btn__primary card">Read More</a>
                    </div>
                </swiper-slide>
                <swiper-slide>
                    <div class="course__card">
                        <div class="course__card--number">.03</div>
                        <p class="course__card--title">Course <span>03</span></p>
                        <div class="course__card--decorator"></div>
                        <p class="course__card--description">Lorem ipsum dolor sit amet, consectetur adipiscing
                            elit, sed
                            do eiusmod tempor incididunt ut labore et.</p>
                        <a href="" class="btn__primary card">Read More</a>
                    </div>
                </swiper-slide>
                <swiper-slide>
                    <div class="course__card">
                        <div class="course__card--number">.04</div>
                        <p class="course__card--title">Course <span>04</span></p>
                        <div class="course__card--decorator"></div>
                        <p class="course__card--description">Lorem ipsum dolor sit amet, consectetur adipiscing
                            elit, sed
                            do eiusmod tempor incididunt ut labore et.</p>
                        <a href="" class="btn__primary card">Read More</a>
                    </div>
                </swiper-slide>
            </swiper>
            <div class="course__swiper--controls">
                <button class="btn__swiper course__swiper--prev">
                    <img src="@/assets/images/Arrow-1.png" alt="Flecha Izquierda">
                </button>
                <button class="btn__swiper course__swiper--next">
                    <img src="@/assets/images/Arrow-2.png" alt="Flecha Derecha">
                </button>
            </div>
            <div class="course__more">
                <p class="course__more--text">more courses</p>
                <button class="btn__swiper more">
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
    name: 'CourseSection',
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
}
</script>
<style lang="scss">
@use '@/assets/styles/components/course.scss';
</style>