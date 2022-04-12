<template>
    <ul>
        <li v-for="(element,index) in homeNav" :key="index">
            <a href="`${element.url}`"> {{element.name}} </a>
        </li>
    </ul>
</template>
<script>
export default {
    name: 'HomeNavComp',
    data () {
        return {
            homeNav : [
                {
                    name: 'characters',
                    url: '/characters'
                },
                {
                    name: 'comics',
                    url: '/comics'
                },
                {
                    name: 'movies',
                    url: '/movies'
                },
                {
                    name: 'tv',
                    url: '/tv'
                },
                {
                    name: 'games',
                    url: '/games'
                },
                {
                    name: 'collectibles',
                    url: '/collectibles'
                },
                {
                    name: 'videos',
                    url: '/videos'
                },
                {
                    name: 'fans',
                    url: '/fans'
                },
                {
                    name: 'news',
                    url: '/news'
                },
                {
                    name: 'shop',
                    url: '/shop'
                },
            ]
        }
    }
}
</script>
<style scoped lang="scss">
//importo scss
@import '../assets/style/mixin.scss'; 

ul {
    @include orizontalMenu;

    li {
        padding: 0 10px;
        text-transform: uppercase;

        a {
            text-decoration: none;
            color: #5e6666;
        }
    }
}

</style>