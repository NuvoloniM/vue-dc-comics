<template>
    <ul>
        <li class="foot-text">follow us</li>
        <li v-for="(element,index) in social" :key="index">
            <a href="`${element.url}`">
                <img :src="`${element.media}`" alt="">
            </a>
        </li>
    </ul>
</template>
<script>
export default {
    name: 'FooterSocialComp',
    data () {
        return {
            social : [
                {
                    media: require('../assets/img/footer-facebook.png'),
                    url: '#',
                },
                {
                    media: require('../assets/img/footer-twitter.png'),
                    url: '#',
                },
                {
                    media: require('../assets/img/footer-youtube.png'),
                    url: '#',
                },
                {
                    media: require('../assets/img/footer-pinterest.png'),
                    url: '#',
                },
                {
                    media: require('../assets/img/footer-periscope.png'),
                    url: '#',
                },
            ]
        }
    }
}
</script>
<style scoped lang="scss">
//importo scss
@import '../assets/style/mixin.scss'; 
@import '../assets/style/variables.scss';

ul {
    @include orizontalMenu;

    li {
        padding: 0 10px;
        text-transform: uppercase;

        a {
            text-decoration: none;
            color: $secondary-color;
            padding: 40px 0;
        }
    }
}

.foot-text {
    color: $primary-color;
    text-transform: uppercase;
    font-weight: bold;
}


</style>