<template>
  <div class="modal block">
    <h2>Добавить новую задачу</h2>
    <form>
      <div>
        <label for="todo">Что нужно сделать?</label>
        <input type="text" id="todo">
      </div>
      <div>
        <div>
          <label for="todoCategories">Категория</label>
          <select id="todoCategories">
            <option>Дом</option>
            <option>Семья</option>
            <option>Работа</option>
            <option>Спорт</option>
          </select>
        </div>
        <div>
          <label for="todoDate">Категория</label>
          <input type="date" id="todoDate">
        </div>
        <div>
        <label for="todoPriority">Категория</label>
        <select id="todoPriority">
          <option>Дом</option>
          <option>Семья</option>
          <option>Работа</option>
          <option>Спорт</option>
        </select>
      </div>
      </div>
    </form>
    <div class="modal__btn">
      <button>Отменить</button>
      <button>Добавить</button>
    </div>
  </div>
</template>

<script>
// export default {
//   name: "TheModal"
// }
</script>

