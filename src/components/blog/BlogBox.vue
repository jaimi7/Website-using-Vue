<script setup lang="ts">
import CommentsFrom from "@components/blog/CommentsFrom.vue"

const categories = [{
    id: 1,
    name: 'Business Analytics',
    count: 23,
}, {
    id: 2,
    name: 'Data Science',
    count: 92,
}, {
    id: 3,
    name: 'Machine Learning',
    count: 39,
}, {
    id: 4,
    name: 'Computer Science',
    count: 50,
}, {
    id: 5,
    name: 'Commerce',
    count: 83,
}, {
    id: 6,
    name: 'Art',
    count: 40,
}, {
    id: 7,
    name: 'Communication',
    count: 72,
}, {
    id: 8,
    name: 'Contact Writing',
    count: 52,
},
]
</script>

<template>
    <div class="blogs">
        <div class="row">
            <div class="blog_left">
                <img src="@/assets/img/certificate.jpg" alt="Certificate">
                <h2>Our Certificate & Online Programs For 2024</h2>
                <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Fuga corporis aperiam consequatur doloribus
                    aut magnam earum porro eaque dolorum ipsam illum, obcaecati voluptate repellendus dolore ratione cum
                    provident possimus illo quod in. Minus cum inventore obcaecati libero, nihil a quisquam!</p>
                <br>
                <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Necessitatibus nesciunt nobis nihil
                    doloremque consequatur nam, fugiat distinctio rem eaque quod facere illo ipsam, esse voluptatum
                    voluptatibus praesentium non. Perspiciatis repudiandae esse voluptatem temporibus provident?
                    Voluptatibus officiis adipisci est repudiandae vero dolores reiciendis veritatis, non sapiente, quo
                    libero cum mollitia voluptatum!</p>
                <br>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Ducimus ipsum, aliquid quae quia quo dolore
                    aut, facere sit repellendus in ullam quam, dolorem iure illum magni commodi quaerat suscipit. Est.
                </p>

                <CommentsFrom />
            </div>
            <div class="blog_right">
                <h3>Post Categories</h3>
                <div v-for="category in categories" :key="category.id">
                    <span>{{ category.name }}</span>
                    <span>{{ category.count }}</span>
                </div>
            </div>
        </div>
    </div>
</template>
