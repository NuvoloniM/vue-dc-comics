<template>
    <div>
        <h2> -- Content goes here -- </h2>
    </div>
</template>
<script>
export default {
    name: 'ContentComp'
}
</script>
<style lang="scss" scoped>

@import '../assets/style/mixin.scss';

    div {
        background: #000;
    
        h2 {
            font-size: 2em;
            color: #fff;
            text-align: start;
            padding: 30px 0;
            @include container
        }
    }
</style>