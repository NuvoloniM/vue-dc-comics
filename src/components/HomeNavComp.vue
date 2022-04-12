<template>
    <ul>
        <li v-for="(element,index) in homeNav" :key="index">
            <a :class="(element.active == true) ? 'active' : '' " href="`${element.url}`"> {{element.name}} </a>
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
                    url: '/characters',
                    active: false,
                },
                {
                    name: 'comics',
                    url: '/comics',
                    active: true,
                },
                {
                    name: 'movies',
                    url: '/movies',
                    active: false,
                },
                {
                    name: 'tv',
                    url: '/tv',
                    active: false,
                },
                {
                    name: 'games',
                    url: '/games',
                    active: false,
                },
                {
                    name: 'collectibles',
                    url: '/collectibles',
                    active: false,
                },
                {
                    name: 'videos',
                    url: '/videos',
                    active: false,
                },
                {
                    name: 'fans',
                    url: '/fans',
                    active: false,
                },
                {
                    name: 'news',
                    url: '/news',
                    active: false,
                },
                {
                    name: 'shop',
                    url: '/shop',
                    active: false,
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

.active {
    color: $primary-color;
    border-bottom: 5px solid $primary-color;
}

</style>