<script>
    export default {
        name: "AppFooter",
        data(){
            return{
                elements:[
                {
                    href: '#',
                    img: 'footer-facebook.png'
                },
                {
                    href: '#',
                    img: 'footer-periscope.png'
                },
                {
                    href: '#',
                    img: 'footer-pinterest.png'
                },
                {
                    href: '#',
                    img: 'footer-twitter.png'
                },
                {
                    href: '#',
                    img: 'footer-youtube.png'
                },
                ]
            }
        },
        methods:{
            getPathImg(imgName){
                return new URL (`../assets/img/${imgName}`, import.meta.url).href
            }
        }
    }
</script>

<template>
  <footer>
    <div class="container">

        <div class="sign-up">
            <a href="#">sign-up now!</a>
        </div>

        <div class="socials">
            <h3>Follow us</h3>
            <ul>
                <li v-for="(element, index) in elements" :key="index">
                    <a href="#">
                        <img :src="getPathImg(element.img)" :alt="element.img">
                    </a>
                </li>
            </ul>
        </div>

    </div>
  </footer>
</template>


<style lang="scss" scoped>
@use '../src/styles/general' as *;
@use '../src/styles/partials/variables' as *;
@use '../src/styles/partials/mixin' as *;

    footer{
        height: 110px;
        width: 100%;
        background-color: #303030;
        .container{
            height: 100%;
            @include centerFlex('vertical');
            justify-content: space-between;
            .sign-up{
                height: 100%;
                min-width: 150px;
                @include centerFlex('vertical');
                    a{
                        color: white;
                        padding: 10px;
                        text-transform: uppercase;
                        border: 2px solid $primary-color;
                        &:hover{
                            background-color: lighten($primary-color, 0%);
                        }
                    }
            }
        }
        .socials{
            @include centerFlex();
            h3{
                text-transform: uppercase;
                color: $primary-color;
                padding-right: 25px;
                font-size: 1rem;
            }
            ul{
                @include centerFlex();
                a:hover img{
                    filter: brightness(160%);
                }
            }
            img{
                margin: 0px 10px;
                min-width: 35px;
            }
        }
    }
</style>