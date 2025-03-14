<template>
    <header class="header">
        <div class="header__container">
            <a href="" class="header__logo">
                <img src="@/assets/images/logo.png" alt="logo-ogilvy">
            </a>
            <div class="header__menu--options desktop">
                <nav>
                    <ul>
                        <li><a href="#">Home</a></li>
                        <li><a href="#">about</a></li>
                        <li><a href="#">courses</a></li>
                        <li><a href="#">blog</a></li>
                        <li><a href="" class="btn">sign in</a></li>
                    </ul>
                </nav>
            </div>
            <button class="header__menu" @click="toggleMenu">
                <img v-if="!isMenuOpen" src="@/assets/images/menu.png" alt="menu-header"> <!-- Ícono de menú -->
                <span v-if="isMenuOpen" class="close-icon">X</span> <!-- Ícono de X -->
            </button>
        </div>
        <!-- Menú con clase activa -->
        <div :class="['header__menu--options', { active: isMenuOpen }]">
            <nav>
                <ul>
                    <li><a href="#">Home</a></li>
                    <li><a href="#">about</a></li>
                    <li><a href="#">courses</a></li>
                    <li><a href="#">blog</a></li>
                    <li><a href="" class="btn">sign in</a></li>
                </ul>
            </nav>
        </div>
    </header>

</template>
<script>
export default {
    name: 'HeaderSection',
    data() {
        return {
            isMenuOpen: false
        };
    },
    methods: {
        toggleMenu() {
            this.isMenuOpen = !this.isMenuOpen;
        }
    }
}
</script>
<style lang="scss">
@use '@/assets/styles/layouts/header.scss';
</style>