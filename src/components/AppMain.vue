<script>

import AppCards from '../components/AppCards.vue'
import cards from '../data/dc-comics'


    export default {
        name: "AppMain",
        components:{
            AppCards
        },
        data(){
            return{
                cards
            }
        }
    }
</script>

<template>
    <main>
        <div class="container">
            <AppCards v-for="(card, index) in cards" :key="index" 
            :cardImg="card.thumb" 
            :cardTitle="card.series"/>
        </div>
    </main>
    
</template>


<style lang="scss" scoped>
@use '../src/styles/general' as *;
@use '../src/styles/partials/variables' as *;
@use '../src/styles/partials/mixin' as *;

    .container{
        display: flex;
        justify-content: center;
        height: 100%;
        gap: 25px;
        flex-wrap: wrap ;
    }
    main{
        background-color:#1c1c1c;
        padding-top: 50px;
        padding-bottom: 80px;
        color: white;
    }
</style>