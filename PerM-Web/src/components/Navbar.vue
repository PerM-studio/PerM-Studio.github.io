<template>
    <div>
        <img @click="compToShow('yt')" src="../assets/images/perm.png" alt="/M logó" class="nav-logo">
        <a @click="compToShow('home')">Rólunk</a>
        <a @click="compToShow('news')">Újdonságok</a>
        <a @click="compToShow('popdubs')">Népszerű szinkronok</a>
        <a @click="compToShow('contact')">Elérhetőségeink</a>
        <a @click="compToShow('other')">Egyéb oldalaink</a>
    </div>
</template>
<script>
import { ref } from 'vue';

var comp = ref("");

function compToShow(compName){
    comp.value = compName;
}

</script>
<script>
import Content from './Content.vue';

    export default{
        components:{Content},
        data(){
            return {comp: ""};
        },
    }
</script>
<style>
    .nav-logo{
        width: 55px;
        height: 55px;
    }
</style>