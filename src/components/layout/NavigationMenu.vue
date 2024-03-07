<script setup lang="ts">
import { RouterLink } from 'vue-router'
const navLinks: HTMLElement | null = document.getElementById("nav_link");

function hideMenu() {
    navLinks.style.right = "0";
}

function showMenu() {
    navLinks.style.right = "-200px";
}

</script>

<template>
    <nav>
        <!-- logo -->
        <RouterLink to="/">
            <img src="@/assets/img/logo.png" alt="Logo" />
        </RouterLink>
        <!-- menus -->
        <div id="nav_link" class="nav_links">
            <i class="fa fa-times" @click="hideMenu()"></i>
            <ul>
                <li>
                    <RouterLink to="/">Home</RouterLink>
                </li>
                <li>
                    <RouterLink to="/about">About</RouterLink>
                </li>
                <li>
                    <RouterLink to="/course">Course</RouterLink>
                </li>
                <li>
                    <RouterLink to="/blog">Blog</RouterLink>
                </li>
                <li>
                    <RouterLink to="/contact">Contact</RouterLink>
                </li>
            </ul>
        </div>
        <i class="fa fa-bars" @click="showMenu()"></i>
    </nav>
</template>
