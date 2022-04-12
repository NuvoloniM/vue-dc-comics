<template>
    <div class="footnav">
        <div>
            <DcComicsMenu/>
            <ShopMenu/>  
        </div>
        <div>
            <DCFootNav/>
        </div>
        <div>
            <SitesNav/>
        </div>
    </div>
</template>
<script>

import DcComicsMenu from './DcComicsMenu.vue';
import ShopMenu from './ShopMenu.vue';
import DCFootNav from './DCFootNav.vue';
import SitesNav from './SitesNav.vue';

export default {
    name: 'FooterNavComp',
    components: {
        DcComicsMenu,
        ShopMenu,
        DCFootNav,
        SitesNav,
    },
}
</script>
<style lang="scss" scoped>

.footnav {
    display: flex;
    align-items: flex-start;
}

</style>