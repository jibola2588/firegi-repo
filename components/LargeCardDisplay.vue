<template>
  <div class="container">
    <h4 class="header">
        {{cardSections.title}}
    </h4>
    <p class="snippet">
        {{cardSections.snippet}}
    </p>
    <div class="cards-container">
       <LargeCard
        v-for="cardSection in cardSections.cards" :key="cardSection.id" 
        :cardSection ="cardSection" />
    </div>
  </div>
</template>

<script>
export default {
    name:'LargeCardDisplay',
    props:['cardSections']
}
</script>

<style scoped>
.container{
    margin-top: 6rem;
}
    .header{
        font-weight: 700;
        font-size: 1.5rem;
    }
    .snippet{
        color: grey;
        margin-bottom: 1.5rem;
    }
    .cards-container{
        display: flex;
        justify-content: space-between;
    }
</style>
