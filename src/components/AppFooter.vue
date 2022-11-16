<script>
    export default {
        name: "AppFooter"
    }
</script>

<template>
  <footer>
      
      <div class="main-wrapper">

        <div class="container">

            <nav>
                <ul>
                    <li>
                        <h3>DC COMICS</h3>
                        <a href="#">link</a>
                        <a href="#">link</a>
                        <a href="#">link</a>
                        <a href="#">link</a>
                        <a href="#">link</a>
                        <a href="#">link</a>
                        <a href="#">link</a>
                        <a href="#">link</a>
                      
                    </li>
                    <li>
                        <h3>DC COMICS</h3>
                        <a href="#">link</a>
                        <a href="#">link</a>
                    </li>
                    <li>
                        <h3>DC COMICS</h3>
                        <a href="#">link</a>
                        <a href="#">link</a>
                        <a href="#">link</a>
                        <a href="#">link</a>
                        <a href="#">link</a>
                        <a href="#">link</a>
                        <a href="#">link</a>
                        <a href="#">link</a>
                        <a href="#">link</a>
                        <a href="#">link</a>
                        <a href="#">link</a>
                        <a href="#">link</a>
                        <a href="#">link</a>
                        <a href="#">link</a>
                        <a href="#">link</a>
                    </li>
                    <li>
                        <h3>DC COMICS</h3>
                        <a href="#">link</a>
                        <a href="#">link</a>
                        <a href="#">link</a>
                        <a href="#">link</a>
                        <a href="#">link</a>
                        <a href="#">link</a>
                        <a href="#">link</a>
                        <a href="#">link</a>
                        <a href="#">link</a>
                        <a href="#">link</a>
                        <a href="#">link</a>
                        <a href="#">link</a>
                        <a href="#">link</a>
                        <a href="#">link</a>
                        <a href="#">link</a>
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
        height: 370px;
        background-color: #303030;
        .main-wrapper{
            background-image: url('../assets/img/footer-bg.jpg');
            background-repeat: no-repeat;
            background-size: cover;
            .container{
                position: relative;
                background-image:url('../assets/img/dc-logo-bg.png') ;
                background-repeat: no-repeat;

                nav{
                    padding-top: 40px;
                    padding-bottom: 50px;
                    height: 370px;
                    width: 25%;
                    ul{
                        height: 280px;
                        display: flex;
                        flex-grow: 0;
                        flex-direction: column;
                        flex-wrap: wrap;
                        li{
                            display: flex;
                            flex-direction: column;
                            margin-bottom: 18px;

                        }
                    }
                    h3{
                        color:white;
                        text-transform: uppercase;
                        margin-bottom: 18px;
                    }
                    a{
                        font-size: .8rem;
                        color: rgb(182, 182, 182);
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