<script>
    export default {
        name: "AppHeader"
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
                    <li><a href="#">Charaters</a></li>
                    <li><a class="active" href="#">comics</a></li>
                    <li><a href="#">movies</a></li>
                    <li><a href="#">tv</a></li>
                    <li><a href="#">games</a></li>
                    <li><a href="#">collectibles</a></li>
                    <li><a href="#">videos</a></li>
                    <li><a href="#">fans</a></li>
                    <li><a href="#">news</a></li>
                    <li><a href="#">shop</a></li>
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
        }
        ul{
            @include centerFlex();
        }
        a{
            color: #464646;
            font-weight: 500;
            font-size: .8rem;
            text-transform: uppercase;
            margin:0px 15px;
            padding-bottom: 45px;
            padding-top: 50px;

            &:hover,
            &.active{
                color: $main-color;
                border-bottom: 4px solid $main-color;
            }
            
        }
        
    }
    

    
</style>