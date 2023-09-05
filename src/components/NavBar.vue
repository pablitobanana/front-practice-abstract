<script setup>
import { RouterLink } from 'vue-router'

const showMenu = () => {
    const menu_icon = document.getElementById('menu-icon')
    menu_icon.style.display = "none"
    const close_icon = document.getElementById('close-icon')
    close_icon.style.display = "block"
    const navbar = document.querySelector('.navbar')
    navbar.style.height = "17.5rem"
}
const closeMenu = () => {
    const close_icon = document.getElementById('close-icon')
    close_icon.style.display = "none"
    const navbar = document.querySelector('.navbar')
    navbar.style.height = "0rem"
    const menu_icon = document.getElementById('menu-icon')
    menu_icon.style.display = "block"
}

</script>

<template>
    <RouterLink to="/" class="logo">
        <i class="fa-brands fa-vuejs "></i>
        Fake Abstract
    </RouterLink>

    <label for="" class="icons">
        <i class="fa-solid fa-bars" id="menu-icon" @click="showMenu"></i>
        <i class="fa-solid fa-xmark" id="close-icon" @click="closeMenu"></i>
    </label>
    <nav class="navbar">
        <RouterLink to="/" class="nav-links">Logo</RouterLink>
        <RouterLink to="/" class="nav-links">Fake page</RouterLink>
    </nav>
</template>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Nunito+Sans:opsz@6..12&display=swap');

* {
    color: #fff;
    text-decoration: none;
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

.logo {
    font-size: 2em;
    font-weight: 700;
    font-family: 'Nunito Sans', sans-serif;
}

.nav-links {
    font-size: 1.25em;
    margin-left: 2.5rem;
    font-weight: 500;
    font-family: 'Nunito Sans', sans-serif;
}

.icons {
    position: absolute;
    font-size: 2.25em;
    cursor: pointer;
    right: 5%;
    display: none;
}

@media (max-width: 768px) {
    .icons {
        display: inline-flex;
    }

    .icons #close-icon {
        display: none;
    }

    .navbar {
        position: absolute;
        top: 100%;
        left: 0;
        width: 100%;
        height: 0;
        background-color: rgba(100, 100, 100, 1);
        box-shadow: 0 .5rem 1rem rgba(0, 0, 0, .1);
        overflow: hidden;
        transition: .3s ease;
    }

    .navbar .nav-links {
        display: block;
        text-align: center;
        font-size: 1.4rem;
        margin: 1.5rem 0;
    }
}
</style>
