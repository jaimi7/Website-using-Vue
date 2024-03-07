<script setup lang="ts">
const facilities = [{
  id: 1,
  title: "World Class Library",
  img: "library.png",
  detail: "Lorem ipsum dolor sit, amet consectetur adipisicing elit. Deleniti repudiandae quia corrupti eos ducimus quo at delectus nisi harum consequuntur?",
}, {
  id: 2,
  title: "Largest Play Groud",
  img: "basketball.png",
  detail: "Lorem ipsum dolor sit, amet consectetur adipisicing elit. Deleniti repudiandae quia corrupti eos ducimus quo at delectus nisi harum consequuntur?",
}, {
  id: 3,
  title: "Testy and Healthy Food",
  img: "cafeteria.png",
  detail: "Lorem ipsum dolor sit, amet consectetur adipisicing elit. Deleniti repudiandae quia corrupti eos ducimus quo at delectus nisi harum consequuntur?",
},];

function getImageUrl(img) {
  return new URL(`../../assets/img/${img}`, import.meta.url).href
} 
</script>

<template>
  <!-- facilities -->
  <section class="container">
    <h2>Our Facilities</h2>
    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
    <div class="row">
      <div v-for="facility in facilities" :key="facility.id" class="facilities_col">
        <img :src="getImageUrl(facility.img)" alt="Library">
        <h3>{{ facility.title }}</h3>
        <p>{{ facility.detail }}</p>
      </div>
    </div>
  </section>
</template>
