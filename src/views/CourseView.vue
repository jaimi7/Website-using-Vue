<script setup lang="ts">
import SubHeaderMenu from "@components/layout/SubHeaderMenu.vue"
import FooterBox from "@components/layout/FooterBox.vue"
import CourseBox from "@components/home/CourseBox.vue"
import TestimonialsBox from "@components/home/TestimonialsBox.vue"
</script>

<template>
  <div>
    <!-- header  -->
    <SubHeaderMenu heading="Our Courses" />

    <!-- course -->
    <CourseBox />

    <!-- testimonials -->
    <TestimonialsBox />

    <!-- footer  -->
    <FooterBox />
  </div>
</template>
