<template>
  <div class="container">
    <Header />
    <Authorization />
    <Footer />
  </div>
</template>

<script setup>
import '../assets/style/app.scss'
import Header from '../components/TheHeader.vue'
import Authorization from "../components/TheAuthorization.vue";
import Footer from "../components/TheFooter.vue";
</script>
