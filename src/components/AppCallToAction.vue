<script>
    export default {
        name: "AppCallToAction",
        data(){
            return{
                elements:[
                {
                    text: 'digital comics',
                    href: '#',
                    img: 'buy-comics-digital-comics.png'
                },
                {
                    text: 'dc merchandise',
                    href: '#',
                    img: 'buy-comics-merchandise.png'
                },
                {
                    text: 'subscription',
                    href: '#',
                    img: 'buy-comics-subscriptions.png'
                },
                {
                    text: 'comic shop locator',
                    href: '#',
                    img: 'buy-comics-shop-locator.png'
                },
                {
                    text: 'dc power visa',
                    href: '#',
                    img: 'buy-dc-power-visa.svg'
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

  <section>
    <div class="container">

        <nav>
            <ul>
                <li v-for="(element, index) in elements" :key="index" >
                    <a href="#">
                        <div class="image">
                            <img :src="getPathImg(element.img)" :alt="element.img">
                        </div>
                        <div class="text">
                            <span>{{element.text}}</span>
                        </div>
                    </a>
                </li>
            </ul>
        </nav>
        
    </div>
  </section>

</template>


<style lang="scss" scoped>
@use '../src/styles/general' as *;
@use '../src/styles/partials/variables' as *;
@use '../src/styles/partials/mixin' as *;

    section{
        background-color: $primary-color;
        height: 150px;
        .container{
            height: 100%;
            @include centerFlex('vertical');
            justify-content: center;
            nav{
                width: 100%;
                ul{
                    @include centerFlex('vertical');
                    
                    li{
                        width:calc(100% / 5);
                        min-width: 155px;
                        a{
                            @include centerFlex('both');
                            color: white;
                            text-transform: uppercase;
                            &:hover{
                                text-decoration: underline;
                            }
                            img{
                                width: 55px;
                                height: 55px;
                                min-width: 55px;
                                object-fit: scale-down;
                            }
                            .text{
                                margin-left: 3%;
                                font-size: .8rem;
                            }
                        }
                        
                    }
                }
            }
        }
        
    }
</style>