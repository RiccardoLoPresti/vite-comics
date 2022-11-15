<script>
    export default {
        name: "AppFooter"
    }
</script>

<template>
  <footer>
      
      <div class="main-wrapper">

        <div class="container">

            <div class="bg-logo"></div>

            <nav>
                <div class="link">
                    <h3>dc comics</h3>
                    <ul>
                        <li><a href="#">cose</a></li>
                        <li><a href="#">cose</a></li>
                        <li><a href="#">cose</a></li>
                        <li><a href="#">cose</a></li>
                        <li><a href="#">cose</a></li>
                        <li><a href="#">cose</a></li>
                        <li><a href="#">cose</a></li>
                    </ul>
                </div>
                <div class="link">
                    <h3>dc comics</h3>
                    <ul>
                        <li><a href="#">cose</a></li>
                        <li><a href="#">cose</a></li>
                        <li><a href="#">cose</a></li>
                        <li><a href="#">cose</a></li>
                        <li><a href="#">cose</a></li>
                        <li><a href="#">cose</a></li>
                        <li><a href="#">cose</a></li>
                    </ul>
                </div>
                <div class="link">
                    <h3>dc comics</h3>
                    <ul>
                        <li><a href="#">cose</a></li>
                        <li><a href="#">cose</a></li>
                        <li><a href="#">cose</a></li>
                        <li><a href="#">cose</a></li>
                        <li><a href="#">cose</a></li>
                        <li><a href="#">cose</a></li>
                        <li><a href="#">cose</a></li>
                    </ul>
                </div>
                <div class="link">
                    <h3>dc comics</h3>
                    <ul>
                        <li><a href="#">cose</a></li>
                        <li><a href="#">cose</a></li>

                    </ul>
                </div>
                
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
                .bg-logo{
                    background-image:url('../assets/img/dc-logo-bg.png') ;
                    background-size: cover;
                    background-position: center;
                    right: 0;
                    position: absolute;
                    width: 560px;
                    height: 370px;
                }
                nav{
                    z-index: 999;
                    position: relative;
                    padding-top: 50px;
                    padding-bottom: 60px;
                    height: 370px;
                    width: 480px;
                    @include centerFlex('vertical');
                    flex-wrap: wrap;
                    .link{
                        margin-right: 50px;
                        margin-bottom: 20px;

                    }
                    h3{
                        color:white;
                        text-transform: uppercase;
                        margin-bottom: 20px;
                    }
                    a{
                        font-size: .8rem;
                        color: rgb(182, 182, 182);
                    }
                }
                .sign-up{
                    height: 110px;
                }
            }
        }
    }
</style>