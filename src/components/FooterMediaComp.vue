<template>
    <div>
        <div>
            <FooterBtn/>
        </div>
        <div>
            <FooterSocialComp/>
        </div>
    </div>
</template>
<script>

import FooterBtn from './FooterBtn.vue';
import FooterSocialComp from './FooterSocialComp.vue'

export default {
    name: 'FooterMediaComp',
    components: {
        FooterBtn,
        FooterSocialComp
    }
}
</script>
<style scoped lang="scss">
@import '../assets/style/mixin.scss';

div {
    @include container;
    display: flex;
    justify-content: space-between;
    align-items: center;
}

</style>