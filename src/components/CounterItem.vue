<template>
    <div class="counter__item">
        <div class="counter__count">
            <p class="counter__plus">+</p>
            <p class="counter__number">{{ count }}</p>
        </div>
        <div class="counter__description">
            <p class="counter__text">{{ title }}</p>
            <p class="counter__text type-01">{{ subtitle }}</p>
        </div>
    </div>
</template>

<script>
export default {
    name: 'CounterItem',
    props: {
        count: {
            type: Number,
            required: true
        },
        title: {
            type: String,
            required: true
        },
        subtitle: {
            type: String,
            required: true
        }
    }
};
</script>

<style lang="scss">
// @use '@/assets/styles/components/counter-item.scss';
</style>