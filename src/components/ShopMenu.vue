<template>
<div>
    <h2>Shop</h2>
    <ul>
        <li v-for="(element,index) in shop" :key="index">
            <a href="`${element.link}`"> {{element.name}}</a>
        </li>
    </ul>
</div>
    
</template>
<script>
export default {
    name: 'ShopMenu',
    data() {
        return {
           shop: [
                {
                    name: 'Shop DC',
                    link: '#',
                },
                {
                    name: 'Shop DC Collectibles',
                    link: '#',
                },
            ] 
        }
    }    
}
</script>
<style lang="scss" scoped>
@import '../assets/style/variables.scss';

h2 {
    color: #fff;
    text-transform: uppercase;
}

ul {
    list-style-type: none;
    padding: 0;
}

a {
    color: $secondary-color;
    text-decoration: none;
}
</style>