<script>
    export default {
        name: "AppCallToAction"
    }
</script>

<template>

  <section>
    <div class="container">
        <img src="../assets/img/buy-comics-digital-comics.png" alt="">
        <img src="../assets/img/buy-comics-merchandise.png" alt="">
        <img src="../assets/img/buy-comics-shop-locator.png" alt="">
        <img src="../assets/img/buy-comics-subscriptions.png" alt="">
        <img src="../assets/img/buy-dc-power-visa.svg" alt="">
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
            @include centerFlex('both');
            img{
                width: 80px;
            }
        }
    }

</style>