<template>
    <section class="accept">
        <div class="accept__container">
            <div class="accept__container--type-02">
                <p class="accept__text">Accept <br>
                    <span>new</span><br>
                    challenges
                </p>
            </div>
            <div class="accept__container--type-03">
                <p class="accept__text type-02">explore</p>
                <div class="accept__arrow"></div>
                <p class="accept__text type-02">about</p>
            </div>
            <div class="accept__decorator">
                <div class="accept__square"></div>
                <p class="accept__text type-03">discover your skills</p>
            </div>
            <div class="accept__decorator type-02">
                <div class="accept__square"></div>
                <p class="accept__text type-03">discover your skills</p>
            </div>
        </div>
    </section>
</template>
<script>
export default {
    name: 'AcceptSection'
}
</script>
<style lang="scss">
@use '@/assets/styles/components/accept.scss';
</style>