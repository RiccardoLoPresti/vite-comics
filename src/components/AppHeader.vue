<script>
    export default {
        name: "AppHeader",
        data(){
        return{
            menu:[
                {
                    text: 'Charaters',
                    href: '#',
                    current: false
                },
                {
                    text: 'comics',
                    href: '#',
                    current: true
                },
                {
                    text: 'movies',
                    href: '#',
                    current: false
                },
                {
                    text: 'tv',
                    href: '#',
                    current: false
                },
                {
                    text: 'games',
                    href: '#',
                    current: false
                },
                {
                    text: 'collectibles',
                    href: '#',
                    current: false
                },
                {
                    text: 'videos',
                    href: '#',
                    current: false
                },
                {
                    text: 'fans',
                    href: '#',
                    current: false
                },
                {
                    text: 'news',
                    href: '#',
                    current: false
                },
                {
                    text: 'shop',
                    href: '#',
                    current: false
                },
            ]
        }
  }
    }
</script>

<template>
    <header>

        <div class="container">

            <div class="logo">
                <img src="/dc-logo.png" alt="DC Logo">
            </div>

            <nav>
                <ul>
                    <li v-for="(link, index) in menu" :key="index">
                        <a :class="{'active': link.current}" href="#">{{link.text}}</a>
                    </li>
                </ul>
        
            </nav>

        </div>
      
    </header>
</template>


<style lang="scss" scoped>
@use '../src/styles/general' as *;
@use '../src/styles/partials/variables' as *;
@use '../src/styles/partials/mixin' as *;

    .container{
        height: 115px;
        @include centerFlex('vertical');
        justify-content: space-between;
        .logo img{
            width: 80px;
            min-width: 40px;
        }
        ul{
            @include centerFlex();
            flex-wrap: wrap;
        }
        a{
            color: #464646;
            font-weight: 500;
            font-size: .8rem;
            text-transform: uppercase;
            margin:0px 15px;
            padding-bottom: 45px;
            padding-top: 40px;

            &:hover,
            &.active{
                color: $primary-color;
                border-bottom: 4px solid $primary-color;
            }
            
        }
        
    }
</style>