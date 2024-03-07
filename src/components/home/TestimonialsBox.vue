<script setup lang="ts">
const testimonials = [{
  id: 1,
  name: "Christine Berkley",
  img: "user1.jpg",
  detail: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Sunt, modi? Harum similique, architecto recusandae alias debitis unde hic omnis sequi corrupti, dolores reprehenderit officia nulla at impedit dignissimos possimus veniam!",
}, {
  id: 2,
  name: "David Byer",
  img: "user2.jpg",
  detail: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Sunt, modi? Harum similique, architecto recusandae alias debitis unde hic omnis sequi corrupti, dolores reprehenderit officia nulla at impedit dignissimos possimus veniam!",
},];

function getImageUrl(img) {
  return new URL(`../../assets/img/${img}`, import.meta.url).href
} 
</script>

<template>
  <!-- testimonials -->
  <section class="container">
    <h2>What Our Student Says</h2>
    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
    <div class="row">
      <div v-for="testimonial in testimonials" :key="testimonial.id" class="testimonials_col">
        <img :src="getImageUrl(testimonial.img)" alt="Christine Berkley">
        <div>
          <p>{{ testimonial.detail }}</p>
          <h3>{{ testimonial.name }}</h3>
          <i class="fa fa-star"></i>
          <i class="fa fa-star"></i>
          <i class="fa fa-star"></i>
          <i class="fa fa-star"></i>
          <i class="fa fa-star-o"></i>
        </div>
      </div>
    </div>
  </section>
</template>
