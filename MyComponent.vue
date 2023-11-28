<template>
  <div>
    <h2>{{ message }}</h2>
    <button @click="changeMessage"> Изменить сообщение</button>
  </div>
</template>

<script>
export default {
  data() {
    return {
      message: 'Привет, мир!'
    };
  },
  methods: {
    changeMessage() {
      this.message = 'Сообщение изменено!';
    }
  }
};
</script>

<style scoped>
/* Стили, специфичные для этого компонента */
</style>

