<template>
  <div class="mainContent">
    <div class="column">
      <Successes />
      <TaskTracker />
    </div>
    <div class="column">
      <TheDate />
      <Notice />
      <Fact />
    </div>
  </div>
</template>

<script setup>
import Successes from './TheSuccesses.vue'
import TheDate from './TheDate.vue'
import Notice from './TheNotice.vue'
import Fact from './TheFact.vue'
import TaskTracker from './TaskTracker.vue'
// <!--export default {-->
// <!--  name: "MainContent"-->
// <!--}-->
</script>

