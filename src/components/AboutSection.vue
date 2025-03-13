<template>
    <section class="aboutus">
        <div class="aboutus__container">
            <div class="aboutus__container--type-02">
                <h2 class="aboutus__title">About <span>us.</span></h2>
                <p class="aboutus__text">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor
                    incididunt ut labore et dolore magna aliqua Quis ipsum suspendisse.</p>
                    <div class="aboutus__container--type-04">
                        <div class="aboutus__container--type-05">
                            <div class="aboutus__square"></div>
                            <p class="aboutus__text">Lorem ipsum dolor.</p>
                        </div>
                        <div class="aboutus__container--type-05">
                            <div class="aboutus__square"></div>
                            <p class="aboutus__text">Lorem ipsum dolor.</p>
                        </div>
                        <div class="aboutus__container--type-05">
                            <div class="aboutus__square"></div>
                            <p class="aboutus__text">Lorem ipsum dolor.</p>
                        </div>
                        <div class="aboutus__container--type-05">
                            <div class="aboutus__square"></div>
                            <p class="aboutus__text">Lorem ipsum dolor.</p>
                        </div>
                    </div>
                <a href="" class="btn__primary">Read More</a>
            </div>
            <div class="aboutus__container--type-03">
                <img src="@/assets/images/hombre-posando-circulo.png" alt="hombre-posando-circulo">
            </div>
            <div class="aboutus__circle"></div>
            <div class="aboutus__circle type-02"></div>
            <div class="aboutus__decorator"></div>
            <div class="aboutus__decorator type-02"></div>

        </div>
    </section>
</template>
<script>
export default {
    name: 'AboutSection'
}
</script>
<style lang="scss">
@use '@/assets/styles/components/aboutus.scss';
</style>