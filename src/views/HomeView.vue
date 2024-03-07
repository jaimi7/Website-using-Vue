<script setup lang="ts">
import HeaderMenu from "@components/layout/HeaderMenu.vue"
import CourseBox from "@components/home/CourseBox.vue"
import CampusBox from "@components/home/CampusBox.vue"
import FacilitiesBox from "@components/home/FacilitiesBox.vue"
import TestimonialsBox from "@components/home/TestimonialsBox.vue"
import ContactUsBox from "@components/home/ContactUsBox.vue"
import FooterBox from "@components/layout/FooterBox.vue"
</script>

<template>
  <div>
    <!-- Header -->
    <HeaderMenu />

    <!-- course -->
    <CourseBox />

    <!-- campus -->
    <CampusBox />

    <!-- facilities -->
    <FacilitiesBox />

    <!-- testimonials -->
    <TestimonialsBox />

    <!-- contact us -->
    <ContactUsBox />

    <!-- Footer  -->
    <FooterBox />
  </div>
</template>
