<template>
<div>
    <h2>Sites</h2>
    <ul>
        <li v-for="(element,index) in sites" :key="index">
            <a href="`${element.link}`"> {{element.name}}</a>
        </li>
    </ul>
</div>
    
</template>
<script>
export default {
    name: 'SitesNav',
    data() {
        return {
           sites: [
                {
                    name: 'DC',
                    link: '#',
                },
                {
                    name: 'MAD Magazine',
                    link: '#',
                },
                {
                    name: 'DC Kids',
                    link: '#',
                },
                {
                    name: 'DC Universe',
                    link: '#',
                },
                {
                    name: 'DC Power Visa',
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