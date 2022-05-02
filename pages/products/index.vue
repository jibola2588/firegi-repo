<template>
   <div>
        <div class="container mt-4"> 
        <LargeCardDisplay
        v-for="cardInfo in largeCardInfo.slice(0,1)" :key="cardInfo.id" 
        :cardSections ="cardInfo" />

        <SmallCardDisplay
        v-for="cardInfo in smallCardInfo.slice(0,1)" :key="cardInfo.id" 
        :cardSection ="cardInfo" />
    </div>
   </div>
</template>

<script>
import { largeCardSections, smallCardSections} from '@/assets/data.js'
    export default {
        data(){ 
            return{ 
                largeCardInfo:largeCardSections,
                smallCardInfo:smallCardSections,
            }
        }
    }
</script>

<style scoped>
.container{
    margin-top: 6rem;
}
</style>