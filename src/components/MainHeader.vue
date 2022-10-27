<template>
  <header class="mainHeader">
    <button class="btn__icon mainHeader__newTask">
      <svg width="20" height="20" viewBox="0 0 20 20" fill="none" xmlns="http://www.w3.org/2000/svg">
        <path d="M10 19C14.9706 19 19 14.9706 19 10C19 5.02944 14.9706 1 10 1C5.02944 1 1 5.02944 1 10C1 14.9706 5.02944 19 10 19Z" stroke="#FAFAFA" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
        <path d="M10 6.3999V13.5999" stroke="#FAFAFA" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
        <path d="M6.40002 10H13.6" stroke="#FAFAFA" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
      </svg>
      Новая задача
    </button>
    <AddToDo />
    <button class="theme">
      <svg width="25" height="24" viewBox="0 0 25 24" fill="none" xmlns="http://www.w3.org/2000/svg">
      <g opacity="0.7">
        <path d="M21.5 12.79C21.3427 14.4922 20.7039 16.1144 19.6582 17.4668C18.6126 18.8192 17.2035 19.8458 15.5957 20.4265C13.9879 21.0073 12.248 21.1181 10.5795 20.7461C8.91102 20.3741 7.38299 19.5345 6.17423 18.3258C4.96546 17.117 4.12594 15.589 3.75391 13.9205C3.38188 12.252 3.49272 10.5121 4.07346 8.9043C4.6542 7.29651 5.68083 5.88737 7.03321 4.84175C8.3856 3.79614 10.0078 3.15731 11.71 3C10.7134 4.34827 10.2338 6.00945 10.3585 7.68141C10.4832 9.35338 11.2039 10.9251 12.3894 12.1106C13.5749 13.2961 15.1466 14.0168 16.8186 14.1415C18.4906 14.2662 20.1517 13.7866 21.5 12.79V12.79Z" stroke="#282846" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
      </g>
      </svg>
    </button>
    <div class="mainHeader__user">
      <p>Хорошего дня, username</p>
      <img src="../assets/image/header__avatar.png" width="46" height="46" alt="avatar">
      <div class="header__menu--wrappper">
        <button @click="showDropdown">
          <svg width="14" height="8" viewBox="0 0 14 8" fill="none" xmlns="http://www.w3.org/2000/svg">
          <path d="M1 1L7 7L13 1" stroke="#29A19C" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
          </svg>
        </button>
        <div class="header__dropdown mainHeader__menu">
          <ul v-if="isShowDropdown">
            <li><a href="#"><img src="../assets/icon/user.png" width="18" height="18" alt="user">Личный кабинет</a></li>
            <li><a href="#"><img src="../assets/icon/menu-moon.png" width="18" height="18" alt="theme">Темный режим</a></li>
            <li><a href="#"><img src="../assets/icon/settings.png" width="18" height="18" alt="settings">Настройки</a></li>
            <li><a href="#" class="premium"><img src="../assets/icon/star.png" width="18" height="18" alt="premium">Премиум</a></li>
            <li><a href="#"><img src="../assets/icon/log-out.png" width="18" height="18" alt="log-out">Выйти</a></li>
          </ul>
        </div>
      </div>
    </div>
  </header>
</template>

<script>
export default {
  name: "MainHeader",
  data: () => ({
    isShowDropdown: false,
  }),
  methods: {
    showDropdown() {
      this.isShowDropdown = !this.isShowDropdown
    },
  },
}
</script>
<script setup>
import AddToDo from './TheModal.vue'
</script>