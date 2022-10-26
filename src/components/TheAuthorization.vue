<template>
  <div class="authorization">
    <div class="authorization--wrapper">
      <h2 class="authorization__title">Вход в аккаунт</h2>
      <div class="authorization__email">
        <input type="email" placeholder="E-mail">
      </div>
      <div class="authorization__pass">
        <input type="password" placeholder="Пароль">
      </div>
      <button class="btn authorization__btn">Войти</button>
      <p class="authorization__registration">Еще нет аккаунта? <a href="#">Регистрация</a></p>
      <div class="authorization__hr">
        <hr>
        <p>или</p>
      </div>
      <div class="authorization__alternative">
        <a href="#"><img src="../assets/icon/vk.png" width="32" height="32" alt="vk"></a>
        <a href="#"><img src="../assets/icon/google.png" width="32" height="32" alt="google"></a>
      </div>
    </div>
  </div>
</template>

<!--<script>-->
<!--export default {-->
<!--  name: "authorization"-->
<!--}-->
<!--</script>-->
