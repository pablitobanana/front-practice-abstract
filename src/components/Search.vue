<script setup>
</script>

<template>
    <div class="container">
        <h1 class="title" >How can we help?</h1>
        <input type="search" class="search" placeholder="Search">
    </div>
</template>

<style scoped>
.container{
   background-color: #dadbf1; 
   display: flex;
   flex-direction: column;
   justify-content: center;
   height: 50vh;
   align-items: center;
}

.container .title{
    text-align: center;
    font-size: 4.5rem; 
    font-family: 'IBM Plex Sans', sans-serif;
}

.container .search{
    height: 4rem;
    font-size: 1.2rem;
    width: 50%;
    padding: 1rem;
    font-family: 'IBM Plex Sans', sans-serif;
}

</style>