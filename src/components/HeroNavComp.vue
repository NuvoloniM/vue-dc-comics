<template>
    <div>
        <HeroShopComp/>
    </div>
</template>
<script>
import HeroShopComp from './HeroShopComp.vue';

export default {
    name: 'HeroNavComp',
    components: {
        HeroShopComp,
    }
}
</script>
<style lang="scss" scoped>
@import '../assets/style/variables.scss';

div {
    background: $primary-color;
}

</style>