<template>
  <div class="main__container">
    <SideBar />
    <div class="main__wrapper">
      <Header />
      <Content />
    </div>
  </div>
</template>

<script setup>
import '../assets/style/app.scss'
import Header from '../components/MainHeader.vue'
import SideBar from '../components/SideBar.vue'
import Content from '../components/MainContent.vue'
</script>