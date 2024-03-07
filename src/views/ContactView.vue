<script setup lang="ts">
import SubHeaderMenu from "@components/layout/SubHeaderMenu.vue"
import FooterBox from "@components/layout/FooterBox.vue"
import ConatctsLocation from "@components/contact-us/ConatctsLocation.vue"
import ContactUs from "@components/contact-us/ContactUs.vue"
</script>

<template>
  <div>
    <!-- header -->
    <SubHeaderMenu heading="Contact Us" />

    <!-- location -->
    <ConatctsLocation />

    <!-- contact us -->
    <ContactUs />

    <!-- footer  -->
    <FooterBox />
  </div>
</template>
