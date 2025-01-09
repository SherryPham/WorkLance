<script setup>
import NavBar from "@/components/NavBar.vue";
import Hero from "@/components/Hero.vue";
import HomeCards from "@/components/HomeCards.vue";
import JobListings from "@/components/JobListings.vue";
</script>
<template>
  <NavBar />
  <Hero />
  <HomeCards />
  <JobListings :limit="3" :showButton="true" />
</template>
