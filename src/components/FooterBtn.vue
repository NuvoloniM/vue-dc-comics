<template>
    <div>
        <a href="#">sign-up now!</a>
    </div>
</template>
<script>
export default {
    name: 'FooterBtn'
}
</script>
<style lang="scss" scoped>

@import '../assets/style/variables.scss';

a{
    color: #fff;
    text-transform: uppercase;
    text-decoration: none;
    padding: 10px;
    border: 2px solid $primary-color;
}
</style>