<template>
  <section class="block tasks">
    <div class="block__header">
      <h3>Активные задачи</h3>
      <button class="block__settings">
        <svg width="28" height="7" viewBox="0 0 28 7" fill="none" xmlns="http://www.w3.org/2000/svg">
          <g opacity="0.4">
            <rect y="0.5" width="6" height="6" rx="3" fill="#282846"/>
            <rect x="11" y="0.5" width="6" height="6" rx="3" fill="#282846"/>
            <rect x="22" y="0.5" width="6" height="6" rx="3" fill="#282846"/>
          </g>
        </svg>
      </button>
    </div>
    <div class="tasks__active">
      <div class="task">
        <div class="task__content">
          <input type="checkbox">
          <div class="checkbox_indicator"></div>
          <p>Приготовить вкусный ужин</p>
        </div>
        <div class="task__btn">
          <button><img src="../assets/icon/edit.png" width="18" height="18" alt="edit"></button>
          <button><img src="../assets/icon/trash.png" width="18" height="18" alt="delete"></button>
        </div>
      </div>
    </div>
    <h3>Завершенные задачи</h3>
    <div class="tasks__completed">

    </div>
  </section>
</template>

<script>
// export default {
//   name: "TaskTracker"
// }
</script>