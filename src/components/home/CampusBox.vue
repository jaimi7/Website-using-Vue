<script setup lang="ts">
const campuses = [{
  id: 1,
  title: "London",
  img: "london.png",
}, {
  id: 2,
  title: "New York",
  img: "newyork.png",
}, {
  id: 3,
  title: "Washington",
  img: "washington.png",
},];

function getImageUrl(img) {
  return new URL(`../../assets/img/${img}`, import.meta.url).href
} 
</script>

<template>
  <!-- campus -->
  <section class="container">
    <h2>Our Global Campus</h2>
    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
    <div class="row">
      <div v-for="campus in campuses" :key="campus.id" class="campus_col">
        <img :src="getImageUrl(campus.img)" :alt="campus.title">
        <div class="layer">
          <h3>{{ campus.title }}</h3>
        </div>
      </div>
    </div>
  </section>
</template>
