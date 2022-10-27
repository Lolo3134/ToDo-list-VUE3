<template>
  <div class="backdrop" v-if="isOpen" @click="close">
    <div class="modal block" @click.stop>
      <h2 class="modal__title">Добавить новую задачу</h2>
      <form>
        <div class="input__wrapper">
          <label for="todo">Что нужно сделать?</label>
          <input type="text" id="todo">
        </div>
        <div class="modal__details">
          <div class="input__wrapper">
            <label for="todoCategories">Категория</label>
            <select id="todoCategories">
              <option>Выбрать</option>
              <option>Дом</option>
              <option>Семья</option>
              <option>Работа</option>
              <option>Спорт</option>
            </select>
          </div>
          <div class="input__wrapper">
            <label for="todoDate">Когда?</label>
            <input type="date" id="todoDate">
          </div>
          <div class="input__wrapper">
          <label for="todoPriority">Приоритет задачи</label>
          <select id="todoPriority">
            <option>Выбрать</option>
            <option>Дом</option>
            <option>Семья</option>
            <option>Работа</option>
            <option>Спорт</option>
          </select>
        </div>
        </div>
      </form>
      <div class="modal__btn">
        <button class="btn--danger" @click="close">Отменить</button>
        <button class="btn--primary" @click="confirm">Добавить</button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    isOpen: {
      type: Boolean,
      required: true,
    },
  },
  emits: {
    ok: null,
    close: null,
  },
  methods: {
    // handleKeydown(e) {
    //   if (this.isOpen && e.key === "Escape") {
    //     this.close();
    //   }
    // },

    close() {
      this.$emit("close");
    },
    confirm() {
      this.$emit("ok");
    },
  },
};
</script>

