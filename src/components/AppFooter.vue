<script>
    export default {
        name: "AppFooter",
        data(){
            return{
                objetcs:[
                {
                    title: 'DC Comics',
                    links: [
                        {
                            href: '#',
                            text: 'Characters',
                        },
                        {
                            href: '#',
                            text: 'Comics',
                        },
                        {
                            href: '#',
                            text: 'Movies'
                        },
                        {
                            href: '#',
                            text: 'TV',
                        },
                        {
                            href: '#',
                            text: 'Games',
                        },
                        {
                            href: '#',
                            text: 'Videos',
                        },
                        {
                            href: '#',
                            text: 'Newss',
                        },
                    ],
                },
                {
                    title: 'Shop',
                    links: [
                        {
                            href: '#',
                            text: 'Shop DC',
                        },
                        {
                            href: '#',
                            text: 'Shop DC Collectibles',
                        }
                    ],
                },
                {
                    title: 'Dc',
                    links: [
                        {
                            href: '#',
                            text: 'Terms Of Use',
                        },
                        {
                            href: '#',
                            text: 'Privacy policy(new)',
                        },
                        {
                            href: '#',
                            text: 'Ad Choices',
                        },
                        {
                            href: '#',
                            text: 'Adevertaising',
                        },
                        {
                            href: '#',
                            text: 'Jobs',
                        },
                        {
                            href: '#',
                            text: 'Subscriptions',
                        },
                        {
                            href: '#',
                            text: 'Talent Workshops',
                        },
                        {
                            href: '#',
                            text: 'CPSC Certificates',
                        },
                        {
                            href: '#',
                            text: 'Ratings',
                        },
                        {
                            href: '#',
                            text: 'Shop Help',
                        },
                        {
                            href: '#',
                            text: 'Contac Us',
                        }
                    ],
                },
                {
                    title: 'Sites',
                    links: [
                        {
                            href: '#',
                            text: 'DC',
                        },
                        {
                            href: '#',
                            text: 'MAD Magazine',
                        },
                        {
                            href: '#',
                            text: 'DC Kids',
                        },
                        {
                            href: '#',
                            text: 'DC Universe',
                        },
                        {
                            href: '#',
                            text: 'DC Power Visa',
                        }
                    ],
                },
                ]
            }
        }
    }
</script>

<template>
  <footer>
      
      <div class="main-wrapper">

        <div class="container">

            <nav>
                <ul>

                    <li v-for="(objetc, index) in objetcs" :key="index">
                        <h3>{{objetc.title}}</h3>
                        <a v-for="(link, index) in objetc.links" :key="index" href="#">{{link.text}}</a>
                    </li>
                    
                </ul>
                
                
            </nav>

        </div>

    </div>
    
    
  </footer>
</template>


<style lang="scss" scoped>
@use '../src/styles/general' as *;
@use '../src/styles/partials/variables' as *;
@use '../src/styles/partials/mixin' as *;

    footer{
        width: 100%;
        height: 370px;
        background-color: #303030;
        .main-wrapper{
            width: 100%;
            background-image: url('../assets/img/footer-bg.jpg');
            background-repeat: no-repeat;
            background-size: cover;
            .container{
                background-image:url('../assets/img/dc-logo-bg.png') ;
                background-repeat: no-repeat;
                background-position:right ;
                nav{
                    width: 100%;
                    padding-top: 37px;
                    padding-bottom: 0px;
                    height: 370px;
                    width: 40%;
                    ul{
                        height: 300px;
                        display: flex;
                        flex-grow: 0;
                        flex-direction: column;
                        flex-wrap: wrap;
                        li{
                            display: flex;
                            flex-direction: column;
                            margin-right: 10px;
                        }
                    }
                    h3{
                        color:white;
                        text-transform: uppercase;
                        margin: 13px 0; 
                        font-size: 1.2rem;
                    }
                    a{
                        font-size: .8rem;
                        margin: 3px 0px;
                        color: rgb(151, 151, 151);
                        &:hover{
                            text-decoration: underline;
                        }
                    }
                }
                .sign-up{
                    height: 110px;
                }
            }
        }
    }
</style>