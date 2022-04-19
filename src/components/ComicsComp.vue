<template>
    <li>
        <a href="#">
        <img :src="img" alt="#">
        <h4> {{ title }}</h4>
        </a>
    </li>
</template>
<script>
export default {
    name: 'ComicsComp',
    props: {
        img: String,
        title: String,
    }
}
</script>
<style lang="scss" scoped>

@import '../assets/style/mixin.scss';
li {
    flex-basis: calc( 100% / 6 );
    padding-right: 10px;
    margin: 10px 0;
    img {
        width: 100%;
    }
    a{
        text-decoration: none;
        color: #fff;
    }
    h4 {
        text-transform: uppercase;
    }
}

</style>