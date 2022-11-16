<script>
    export default {
    name:"AppJumbo"
    }
</script>

<template>
  <div class="jumbo"></div>
  <div class="container">
    <p>Current Series</p>
  </div>
</template>


<style lang="scss" scoped>
@use '../src/styles/partials/variables' as *;
@use '../src/styles/general' as *;
.jumbo{
    background-image: url('../assets/img/jumbotron.jpg');
    background-repeat: no-repeat;
    background-size: cover;
    height: 400px;
}
.container{
  position: relative;
}
p{
  position: absolute;
  left: 40px;
  bottom: -27px;
  border: none;
  background-color: $primary-color;
  width: 250px;
  height: 55px;
  text-align: center;
  line-height: 55px;
  color: white;
  text-transform: uppercase;
  font-weight: 500;
  font-size: 1.3rem;
}
</style>