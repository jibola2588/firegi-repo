<template>
    <div class="container" >
   <MyItem 
   v-for="(item,index) in myRentals" :key="index"
   :item="item"/>
    </div>
</template>

<script>
import {mapState} from 'vuex'
    export default {
        layout:'no-nav',
        computed:{ 
            ...mapState(['myRentals'])
        }
    }
</script>

<style  scoped>

</style>