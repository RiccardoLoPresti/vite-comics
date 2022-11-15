<script>
    export default {
        name: "AppCallToAction"
    }
</script>

<template>

  <section>
    <div class="container">
        <nav>
            <ul>
                <li>
                    <a href="#">
                        <div class="image">
                            <img src="../assets/img/buy-comics-digital-comics.png" alt="">
                        </div>
                        <div class="text">
                            <span>digital comics</span>
                        </div>
                    </a>
                    <a href="#">
                        <div class="image">
                            <img src="../assets/img/buy-comics-merchandise.png" alt="">
                        </div>
                        <div class="text">
                            <span>dc merchandise</span>
                        </div>
                    </a>
                    <a href="#">
                        <div class="image">
                            <img src="../assets/img/buy-comics-subscriptions.png" alt="">
                        </div>
                        <div class="text">
                            <span>subscription</span>
                        </div>
                    </a>
                    <a href="#">
                        <div class="image">
                            <img src="../assets/img/buy-comics-shop-locator.png" alt="">
                        </div>
                        <div class="text">
                            <span>comic shop locator</span>
                        </div>
                    </a>
                    <a href="#">
                        <div class="image">
                            <img src="../assets/img/buy-dc-power-visa.svg" alt="">
                        </div>
                        <div class="text">
                            <span>dc power visa</span>
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
            width: 100%;
            @include centerFlex('both');
            li{
                @include centerFlex();
                a{
                    color:white;
                    text-transform: uppercase;
                    width: 100%;
                    padding: 0px 25px; 
                    @include centerFlex();
                    img{
                        width: 55px;
                        min-width: 40px;
                        height: 55px;
                        object-fit:scale-down;
                    }
                    .text{
                        margin-left: 10px;
                    }
                    &:hover{
                        text-decoration: underline;
                    }
                }
            }
            
        }
    }

</style>