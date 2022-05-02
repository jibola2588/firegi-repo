<template>
    <nav class="navbar navbar-expand-lg navbar-dark bg-dark padding sticky mb-5">
    <NuxtLink class="navbar-brand" to="/">Firengii</NuxtLink>
    <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
    </button>

    <div class="collapse navbar-collapse ml-auto" id="navbarSupportedContent">
        <ul class="navbar-nav ml-auto">
            <li class="nav-item active">
                <NuxtLink to="/products" class="nav-link">Products <span class="sr-only">(current)</span></NuxtLink>
            </li>
            <li class="nav-item active">
                <NuxtLink to="/myItems" class="nav-link">My Items <span class="sr-only">(current)</span></NuxtLink>
            </li>
        </ul>
    </div>
    </nav>
</template>

<script>
    export default {
        name:'NuxtNav'
    }
</script>

<style scoped>
    nav{
        z-index:3;
    }
    .padding {
        padding: 1.5rem;
        background-color: black
    }
    .nav-left {
        margin-left: auto;
    }
    .sticky{ 
        position:fixed;
        top:0px;
        width:100%
    }
</style>