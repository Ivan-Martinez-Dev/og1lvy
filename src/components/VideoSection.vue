<template>
    <section class="video">
        <div class="video__container">
            <img src="@/assets/images/video.png" alt="">
            <div class="video__container--decorator">
                <div class="video__icon">
                    <img src="@/assets/images/Arrow-3.png" alt="Imagen Estática" />
                </div>
                <div class="video__text">
                    <p>Ready to</p>
                    <p>get started</p>
                </div>
            </div>
            <div class="video__container--decorator type-02">
                <div class="video__text type-02">
                    <p>Ready to</p>
                    <p>get started</p>
                </div>
                <div class="video__icon">
                    <img src="@/assets/images/Arrow-4.png" alt="Imagen Estática" />
                </div>
            </div>
        </div>

    </section>
</template>
<script>
export default {
    name: 'VideoSection'
}
</script>
<style lang="scss">
@use '@/assets/styles/components/video.scss';
</style>