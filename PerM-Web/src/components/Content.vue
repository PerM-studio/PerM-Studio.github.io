<template>
    <div>
        <Contact v-if="comp == 'contact'"></Contact>
        <Home v-if="comp == 'home'"></Home>
        <News></News>
        <Otherweb></Otherweb>
        <Popdubs></Popdubs>       
    </div>
</template>
<script>
    import Contact from './assets/Contact.vue';
    import Home from './assets/Home.vue';
    import News from './assets/News.vue';
    import Otherweb from './assets/Otherweb.vue';
    import Popdubs from './assets/Popdubs.vue';

    export default{
        props:{
            comp:{
                type: String,
                required: true,
            }
        }
    }
</script>
<style>
    
</style>