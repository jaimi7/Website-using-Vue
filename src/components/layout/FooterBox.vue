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
    <div class="footer">
        <h4>About Us</h4>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Sit impedit incidunt, quaerat, eos inventore
            praesentium <br> aliquid voluptate similique perferendis ea sint nostrum voluptatum ad, est natus fuga
            numquam velit expedita.</p>
        <div class="icons">
            <i class="fa fa-facebook"></i>
            <i class="fa fa-twitter"></i>
            <i class="fa fa-instagram"></i>
            <i class="fa fa-linkedin"></i>
        </div>
        <p>Made with <i class="fa fa-heart-o"></i> by Jaimi !</p>
    </div>
</template>
