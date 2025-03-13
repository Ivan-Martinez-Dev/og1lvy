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

</style>