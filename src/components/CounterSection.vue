<template>
    <section class="counter">
        <div class="counter__container">
            <CounterItem v-for="(item, index) in counterItems" :key="index" :count="item.count" :title="item.title"
                :subtitle="item.subtitle" />
        </div>
    </section>
</template>

<script>
import CounterItem from './CounterItem.vue';  // Componente hijo

export default {
    name: 'CounterSection',
    components: {
        CounterItem
    },
    data() {
        return {
            counterItems: [
                { count: 150, title: 'Happy', subtitle: 'Students' },
                { count: 50, title: 'Certified', subtitle: 'Courses' },
                { count: 1000, title: 'Awards', subtitle: 'Received' }
            ]
        };
    }
};
</script>

<style lang="scss">
@use '@/assets/styles/components/counter.scss';
</style>