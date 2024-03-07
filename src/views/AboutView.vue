<script setup lang="ts">
import SubHeaderMenu from "@components/layout/SubHeaderMenu.vue"
import FooterBox from "@components/layout/FooterBox.vue"
import AboutUs from "@components/AboutUs.vue"
</script>

<template>
  <div>
    <!-- header -->
    <SubHeaderMenu heading="About Us" />

    <!-- about us  -->
    <AboutUs />

    <!-- footer  -->
    <FooterBox />
  </div>
</template>
