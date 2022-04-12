<template>
<div>
    <h2>DC Comics</h2>
    <ul>
        <li v-for="(element,index) in dcComics" :key="index">
            <a href="`${element.link}`"> {{element.name}}</a>
        </li>
    </ul>
</div>
    
</template>
<script>
export default {
    name: 'DcComicsMenu',
    data() {
        return {
           dcComics: [
                {
                    name: 'Characters',
                    link: '#',
                },
                {
                    name: 'Comics',
                    link: '#',
                },
                {
                    name: 'Movies',
                    link: '#',
                },
                {
                    name: 'TV',
                    link: '#',
                },
                {
                    name: 'Games',
                    link: '#',
                },
                {
                    name: 'Videos',
                    link: '#',
                },
                {
                    name: 'News',
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