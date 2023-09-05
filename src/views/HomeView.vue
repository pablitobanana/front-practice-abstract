<script setup>
import NavBar from '../components/MyNavBar.vue';
import Search from '../components/Search.vue';
</script>

<template>
    <header class="header">
      <NavBar />
    </header>
    <main class="main">
      <Search/>
    </main>
</template>

<style scoped> 

* {
   box-sizing: border-box;
 }
 
 .header {
   position: relative;
   top: 0;
   left: 0;
   width: 100%;
   padding: 1.3rem 10%;
   background-color: #000;
   display: flex;
   justify-content: space-between;
   align-items: center;
   z-index: 100;
 }

 @media (max-width: 992px) {
   .header {
     padding: 1.3rem 5%;
   }
 }
</style>