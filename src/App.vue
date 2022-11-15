<script>
    import AppHeader from '../src/components/AppHeader.vue';
    import AppMain from '../src/components/AppMain.vue';
    import AppFooter from '../src/components/AppFooter.vue';

    export default {
        name:"App",
        components:{
            AppHeader,
            AppMain,
            AppFooter
        }
    }
</script>

<template>
    <AppHeader/> 
    <AppMain/> 
    <AppFooter/> 
</template>


<style lang="scss">

@use './src/styles/general' as *;

</style>