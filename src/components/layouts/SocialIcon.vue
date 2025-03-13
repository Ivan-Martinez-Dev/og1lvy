<template>
    <div :class="['footer__icon']">
        <div :class="[`footer__icon--${name}`]" />
    </div>

</template>

<script>
export default {
    name: 'SocialIcon',
    props: {
        name: {
            type: String,
            required: true
        }
    }
};
</script>

<style scoped lang="scss">
// &--facebook {
//   background-image: url('@/assets/icons/facebook.svg');
// }

// &--instagram {
//   background-image: url('@/assets/icons/instagram.svg');
// }

// &--youtube {
//   background-image: url('@/assets/icons/youtube.svg');
// }</style>