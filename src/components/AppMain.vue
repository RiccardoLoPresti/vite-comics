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
            <div class="card-section">
                <AppCards v-for="(card, index) in cards" :key="index" 
                :cardImg="card.thumb" 
                :cardTitle="card.series"/>
            </div>
            
            <div class="button">
                <button>Load More</button>
            </div>
        </div>
    </main>
    
</template>


<style lang="scss" scoped>
@use '../src/styles/general' as *;
@use '../src/styles/partials/variables' as *;
@use '../src/styles/partials/mixin' as *;

    .card-section{
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
    .button{
        text-align: center;
        margin-top: 80px;
        button{
            border: none;
            background-color:$primary-color;
            width: 180px;
            height: 35px;
            color: white;
            text-transform: uppercase;
            font-weight: 600;
            font-size: .8rem;
            cursor: pointer;
            &:hover{
                background-color: lighten($primary-color, 20%);
            }
        }
        
    }
</style>