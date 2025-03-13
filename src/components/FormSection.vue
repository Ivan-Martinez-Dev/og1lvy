<template>
    <section class="form">
        <div class="form__container">
            <img :src="image" alt="Imagen Estática" class="form__img" />
            <div class="form__container--type-02">
                <div class="form__info">
                    <h3 class="form__info--title">Subscribe</h3>
                    <h3 class="form__info--subtitle">to our newsletter</h3>
                    <p class="form__info--text">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
                        eiusmod tempor incididunt .</p>
                </div>
                <form action="" class="form__form">
                    <input type="text" class="form__form--input" placeholder="Name" />
                    <input type="text" class="form__form--input" placeholder="Mail" />
                    <textarea class="form__form--input message" placeholder="Message" />
                    <button class="btn__submit">Send Message</button>
                </form>
            </div>

        </div>
    </section>
</template>
<script>
export default {
    name: 'FormSection',
    data() {
        return {
            image: require('@/assets/images/hombre-manos-footer.png')
        }
    }
};
</script>
<style lang="scss">
@use '@/assets/styles/components/form.scss' as *;
@use '@/assets/styles/components/buttons.scss' as *;
</style>