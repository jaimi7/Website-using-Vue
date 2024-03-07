<script setup lang="ts">
import NavigationMenu from "@components/layout/NavigationMenu.vue";

const props = withDefaults(
  defineProps<{
    heading?: string;
  }>(),
  {
    heading: undefined,
  }
);
</script>

<template>
  <!-- header  -->
  <div class="sub_header">
    <!-- navigation  -->
    <NavigationMenu />
    <!-- main content  -->
    <h1>{{ props.heading }}</h1>
  </div>
</template>
