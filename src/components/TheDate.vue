<template>
  <section class="block">
    <div class="block__header">
      <h3>Такс такс такс</h3>
    </div>
    <div class="date">
      <div>
        <p class="date__title">На часах у нас</p>
        <div class="date__wrapper">
          <img src="../assets/icon/clock.png" width="24" height="24" alt="clock">
          <p>{{ localeTime }}</p>
        </div>
      </div>
      <div>
        <p class="date__title">А сегодня у нас</p>
        <div  class="date__wrapper">
          <img src="../assets/icon/calendar.png" width="24" height="24" alt="calendar">
          <p>{{ localeDate }}</p>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  data: () => ({
    date: new Date,
  }),
  computed: {
    localeDate() {
      return (new Date).toLocaleDateString('ru', {
        year: 'numeric', month: 'long', day: 'numeric', weekday: 'long'
      })
    },
    localeTime() {
      return (new Date).toLocaleTimeString()
    },
  },
  created() {
    this.intervalId = setInterval(() => this.date = Date.now(), 1000); // Обновляем значения не чаще раза в секунду. А то и реже.
  },
}
</script>

