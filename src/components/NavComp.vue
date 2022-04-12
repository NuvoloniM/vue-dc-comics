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
    nav {
        display: flex;
        justify-content: space-between;
        width: 80%;
        margin: 0 auto;
    }
</style>