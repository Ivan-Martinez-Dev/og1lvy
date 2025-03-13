<template>
    <section class="whyus">
        <div class="whyus__container">
            <div class="whyus__container--type-02">
                <img src="@/assets/images/hombre-sentado-circulos.png" alt="">
            </div>
            <div class="whyus__container--type-03">
                <h2 class="whyus__title">Why <span>us.</span></h2>
                <p class="whyus__text">
                    Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore
                    et dolore magna aliqua Quis ipsum suspendisse consectetur adipiscing elit, sed do eiusmod tempor
                    incididunt ut labore et dolore magna aliqua Quis ipsum suspendisse.
                </p>
                <a href="" class="btn__primary">Read More</a>
            </div>
            <p class="whyus__decorator">
                Explore
            </p>
            <div class="whyus__circle"></div>
        </div>

    </section>
</template>
<script>
export default {
    name: 'WhySection'
}
</script>
<style lang="scss">
@use '@/assets/styles/components/whyus.scss';
@use '@/assets/styles/components/buttons.scss';
</style>