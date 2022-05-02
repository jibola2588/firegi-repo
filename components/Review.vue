<template>
    <div class="container">
     <h3 class="mb-2">Customer reviews</h3>
     <div v-if="!$fetchState.pending">
         <ReviewCard  
         v-for="(review,index) in reviewers.results" :key="index"
           :review="review" />
     </div>
     <div v-else>
            fetching data...
     </div>
    </div>
</template>

<script>
    export default {
    data() {
      return {
        reviewers: []
      }
    },
    async fetch() {
      // await fetch(
      //   'https://randomuser.me/api/'
      // ).then(res => res.json())
      // .then(data => { 
      //   console.log(data);
      //   this.reviewers = data;
      // })
      const res = await fetch('https://randomuser.me/api/?results=5');
      const data = await res.json();
      console.log(data);
      this.reviewers = data;
    }
  }
</script>

<style scoped>
</style>