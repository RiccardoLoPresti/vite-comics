<script>
    export default {
        name: "AppFooter"
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
                <li><a href="#"><img src="../assets/img/footer-facebook.png" alt="fb"></a></li>
                <li><a href="#"><img src="../assets/img/footer-facebook.png" alt="fb"></a></li>
                <li><a href="#"><img src="../assets/img/footer-facebook.png" alt="fb"></a></li>
                <li><a href="#"><img src="../assets/img/footer-facebook.png" alt="fb"></a></li>
                <li><a href="#"><img src="../assets/img/footer-facebook.png" alt="fb"></a></li>
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
        background-color: #303030;
        .container{
            height: 100%;
            @include centerFlex('vertical');
            justify-content: space-between;
            .sign-up{
                height: 100%;
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
                margin-right: 20px;
            }
            ul{
                @include centerFlex();
            }
            img{
                margin: 0px 10px;
            }
        }
    }
</style>