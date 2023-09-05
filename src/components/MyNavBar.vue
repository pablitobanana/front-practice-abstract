<script setup>
import { RouterLink } from 'vue-router'
</script>


<template>
    <RouterLink to="/" class="logo">
        <i class="fa-brands fa-vuejs "></i>
        Fake Abstract
    </RouterLink>
    <nav class="navbar">
        <RouterLink to="/" class="btn-navbar-link-grey">Submit a request</RouterLink>
        <RouterLink to="/" class="btn-navbar-link-blue">Sign in</RouterLink>
    </nav>
</template>


<style scoped>
@import url('https://fonts.googleapis.com/css2?family=IBM+Plex+Sans&display=swap');

* {
    color: aliceblue;
    text-decoration: none;
}


.logo {
    font-size: 1.7rem;
    font-family: 'IBM Plex Sans', sans-serif;
}


.btn-navbar-link-grey {
    padding: .4rem 1rem;
    border: .1rem solid #fff;
    border-radius: .5rem;
    background-color: #191A1B;
}

.btn-navbar-link-blue {
    padding: .5rem 2rem;
    border-radius: .5rem;
    background-color: #4D5ED5;
}

.navbar {
    display: flex;
    gap: 1rem;
    width: 33%;
    font-family: 'IBM Plex Sans', sans-serif;
    font-size: 1.5rem;
}

@media (max-width: 992px) {
    .navbar {
        width: 33%;
    }
}
</style>