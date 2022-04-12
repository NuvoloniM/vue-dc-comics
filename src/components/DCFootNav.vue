<template>
<div>
    <h2>DC</h2>
    <ul>
        <li v-for="(element,index) in dc" :key="index">
            <a href="`${element.link}`"> {{element.name}}</a>
        </li>
    </ul>
</div>
    
</template>
<script>
export default {
    name: 'DCFootNav',
    data() {
        return {
           dc: [
                {
                    name: 'Term of Use',
                    link: '#',
                },
                {
                    name: 'Privacy policy(New)',
                    link: '#',
                },
                {
                    name: 'Ad Choices',
                    link: '#',
                },
                {
                    name: 'Advertising',
                    link: '#',
                },
                {
                    name: 'Jobs',
                    link: '#',
                },
                {
                    name: 'Subscription',
                    link: '#',
                },
                {
                    name: 'Talent Workshops',
                    link: '#',
                },
                {
                    name: 'CPSC Certificates',
                    link: '#',
                },
                {
                    name: 'Ratings',
                    link: '#',
                },
                {
                    name: 'Shop Help',
                    link: '#',
                },
                {
                    name: 'Contact Us',
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