<template>
  <div>
    <ul>
      <li v-for="item in menuItems" :key="item.id">
        {{ item.text }}
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "Menu",
  data() {
    return {
      menuItems: [
        { id: 1, text: 'Главная' },
        { id: 2, text: 'О нас' },
        { id: 3, text: 'Контакты' }
      ],
    };
  },
};
</script>

<style scoped>
/* Стили, специфичные для этого компонента */
ul {
  list-style-type: none;
  padding: 0;
  margin: 0;
  display: flex;
  background-color: #eee;
  flex-wrap: wrap; /* Добавляем поддержку переноса элементов на новую строку */
}

li {
  padding: 15px;
  border-right: 1px solid #ccc;
  cursor: pointer;
  flex: 1; /* Распределяем пространство равномерно между элементами */
}

li:last-child {
  border-right: none;
}

/* Добавляем стили для адаптивности */
@media (max-width: 600px) {
  li {
    border-bottom: 1px solid #ccc;
    border-right: none;
  }
}
</style>

