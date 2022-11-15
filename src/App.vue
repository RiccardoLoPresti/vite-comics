<script>
    import AppHeader from '../src/components/AppHeader.vue';
    import AppMain from '../src/components/AppMain.vue';
    import AppCallToAction from '../src/components/AppCallToAction.vue';
    import AppFooter from '../src/components/AppFooter.vue';
    import AppFooterSignIn from '../src/components/AppFooterSignIn.vue';

    export default {
        name:"App",
        components:{
            AppHeader,
            AppMain,
            AppCallToAction,
            AppFooter,
            AppFooterSignIn
        }
    }
</script>

<template>
    <AppHeader/> 
    <AppMain/> 
    <AppCallToAction/> 
    <AppFooter/> 
    <AppFooterSignIn/> 
</template>


<style lang="scss">

@use './src/styles/general' as *;

</style>