<template>
    <NuxtLink  :to="`products/${cardSection.id}`" class="card">
        <img :src="require(`@/assets/images/${cardSection.image}`)" alt="" class="image">
        <h3 class="header">{{cardSection.title}}</h3>
        <p class="snippet">{{cardSection.snippet}}</p>
    </NuxtLink>
</template>

<script>
    export default {
        name:'LargeCard',
        props:['cardSection']
    }
</script>

<style scoped>
  .card {
        width: 31.5%;
        height: 25rem;
        border: none;
        overflow: hidden;
        padding: 0;
        cursor: pointer;
    }
    .image {
        height: 65%;
        border-radius: 0.5rem;
    }
    .header {
        font-size: 1.15rem;
        margin-top: 0.4rem;
        color:black
    }
    a{ 
        text-decoration: none;
    }
    .snippet {
        color: grey;
        text-decoration:none
    }
</style>