<template>
    <ul>
        <li v-for="(element, index) in shop" :key="index">
            <a :href="`${element.link}`">
                <div>
                   <img :src="`${element.media}`" alt=""> 
                </div>
                <div class="text">
                    {{element.name}}
                </div>
            </a>
        </li>
    </ul>
</template>
<script>
export default {
    name: 'HeroShopComp',
    data() {
        return {
            shop: [
                {
                    media: require('../assets/img/buy-comics-digital-comics.png'),
                    name: 'digital comics',
                    link: '#',
                },
                {
                    media: require('../assets/img/buy-comics-merchandise.png'),
                    name: 'dc merchandise',
                    link: '#',
                },
                {
                    media: require('../assets/img/buy-comics-subscriptions.png'),
                    name: 'subscription',
                    link: '#',
                },
                {
                    media: require('../assets/img/buy-comics-shop-locator.png'),
                    name: 'comic shop locator',
                    link: '#',
                },
                {
                    media: require('../assets/img/buy-dc-power-visa.svg'),
                    name: 'dc power visa',
                    link: '#',
                },
            ]
        }
        
    }
}
</script>
<style lang="scss" scoped>
@import '../assets/style/mixin.scss'; 
@import '../assets/style/variables.scss';

ul {
    @include orizontalMenu;
    @include container;
    padding: 30px 0px;

    li {
        padding: 0px;
        text-transform: uppercase;
        flex-basis: calc(100% / 5);

        a {
            text-decoration: none;
            color: #fff;
            display: flex;
            align-items: center;
            text-align: center;
            // padding: 0px 20px;

            div {
                width: calc((100%/2) - 10px);
                margin: 0 5px;

                img {
                    height: 100%;
                }
            }
        }
    }
}
</style>