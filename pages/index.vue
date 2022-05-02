<template>
<div>
  <div class="container">
    <Hero />
    <LargeCardDisplay v-for="cardInfo in largeCardInfo" :key="cardInfo.id"
    :cardSections= "cardInfo"/>
    <SmallCardDisplay 
    v-for="cardSection in smallCardInfo" :key="cardSection.id"
    :cardSection="cardSection" />
  </div>
  </div>
</template>

<script>
import { largeCardSections } from '@/assets/data.js';
import { smallCardSections } from '@/assets/data.js'
export default {
  name: 'IndexPage',
  data(){ 
    return{ 
      largeCardInfo:largeCardSections,
       smallCardInfo:smallCardSections
    }
  }
}
</script>
