<template>
    <nav>
        <LogoComp/>
        <HomeNavComp/>
    </nav>
</template>
<script>
import LogoComp from "./LogoComp.vue";
import HomeNavComp from "./HomeNavComp.vue";

export default {
    name: 'NavComp',
    components: {
        LogoComp,
        HomeNavComp,
    },
}
</script>
<style scoped lang="scss">
@import '../assets/style/mixin.scss';

    nav {
        display: flex;
        justify-content: space-between;
        @include container;
    }
</style>