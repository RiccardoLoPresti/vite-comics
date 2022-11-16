<script>
export default {
    name: "AppCards",
    props:{
        cardImg: String,
        cardTitle: String,
    }
}
</script>

<template>

    <div class="cards">
        <img :src="cardImg" :alt="cardTitle">
        <p>{{cardTitle}}</p>
    </div>
  
</template>


<style lang="scss" scoped>
@use '../src/styles/general' as *;
@use '../src/styles/partials/variables' as *;
@use '../src/styles/partials/mixin' as *;


        
        .cards{
            width: 177px;
            height: 177px;
            margin-bottom: 63px;
        }
        img{
            height: 100%;
            width: 100%;
            object-fit: cover;
            object-position: top;
        }
        p{
            text-transform: uppercase;
            margin-top: 20px;
            font-size: .9rem;
        }

    
</style>