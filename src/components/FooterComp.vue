<template>
    <div>
        <FooterNavComp/>
        <FooterLogo/>
    </div>
</template>

<script>
import FooterNavComp from './FooterNavComp.vue';
import FooterLogo from './FooterLogo.vue';

export default {
    name: 'FooterComp',
    components: {
        FooterLogo,
        FooterNavComp
    }
}
</script>

<style scoped lang="scss">

@import '../assets/style/mixin.scss';

    div {
        display: flex;
        align-items: center;
        justify-content: space-between;
        height: 400px;
        @include container;
        padding: 20px 0;
    }
</style>