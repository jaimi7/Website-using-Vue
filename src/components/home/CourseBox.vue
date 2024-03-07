<script setup lang="ts">
const courses = [{
  id: 1,
  title: "Intermediate",
  detail: "Lorem ipsum dolor sit amet consectetur adipisicing elit. A obcaecati nisi, tempore maiores placeat rerum! Quam qui perspiciatis perferendis? Excepturi totam consequatur necessitatibus corrupti voluptas amet voluptatum dicta iusto labore!",
}, {
  id: 2,
  title: "Degree",
  detail: "Lorem ipsum dolor sit amet consectetur adipisicing elit. A obcaecati nisi, tempore maiores placeat rerum! Quam qui perspiciatis perferendis? Excepturi totam consequatur necessitatibus corrupti voluptas amet voluptatum dicta iusto labore!",
}, {
  id: 3,
  title: "Post Graduation",
  detail: "Lorem ipsum dolor sit amet consectetur adipisicing elit. A obcaecati nisi, tempore maiores placeat rerum! Quam qui perspiciatis perferendis? Excepturi totam consequatur necessitatibus corrupti voluptas amet voluptatum dicta iusto labore!",
},];
</script>

<template>
  <!-- course -->
  <section class="container">
    <h2>Courses We Offer</h2>
    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
    <div class="row">
      <div v-for="course in courses" :key="course.id" class="course_col">
        <h3>{{ course.title }}</h3>
        <p>{{ course.detail }}</p>
      </div>
    </div>
  </section>
</template>
