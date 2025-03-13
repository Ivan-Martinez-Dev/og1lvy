<template>
    <footer class="footer">
        <div class="footer__container">

            <!-- Sección de Enlaces -->
            <FooterLinks :title="'About'" :links="aboutLinks" />

            <FooterLinks :title="'What we do'" :links="whatWeDoLinks" />

            <!-- Sección de Newsletter -->
            <div class="footer__items footer__newsletter">
                <div class="footer__newsletter--title">
                    <h3 class="footer__title type-02">Sign Up To Receive</h3>

                    <h3 class="footer__title type-02"><span>___</span> Our Newsletter</h3>
                </div>
                <div class="footer__newsletter-form">
                    <input type="email" class="footer__input" />
                </div>
                <!-- Sección de Redes Sociales -->
                <div class="footer__follow">
                    <p class="footer__follow--text">Follow us!</p>
                    <SocialIcon name="facebook" />
                    <SocialIcon name="instagram" />
                    <SocialIcon name="youtube" />
                </div>
            </div>
        </div>
    </footer>
</template>

<script>
import FooterLinks from './FooterLinks.vue';  // Componente reutilizable para las secciones de enlaces
import SocialIcon from './SocialIcon.vue';        // Componente reutilizable para los iconos sociales

export default {
    name: 'FooterSection',
    components: {
        FooterLinks,
        SocialIcon
    },
    data() {
        return {
            aboutLinks: [
                { text: 'History', href: '#' },
                { text: 'Our Team', href: '#' },
                { text: 'Mission Statement', href: '#' },
                { text: 'Terms & Condition', href: '#' },
                { text: 'Privacy Policy', href: '#' }
            ],
            whatWeDoLinks: [
                { text: 'News and stories', href: '#' },
                { text: 'Publications', href: '#' },
                { text: 'Take action', href: '#' },
                { text: 'Recommendations', href: '#' },
                { text: 'Help', href: '#' }
            ]
        };
    }
};
</script>

<style lang="scss">
@use '@/assets/styles/layouts/footer.scss';
</style>