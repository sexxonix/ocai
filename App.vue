<template>
  <div id="app">
  <Menu></Menu>
  <MyComponent></MyComponent>
  </div>
</template>

<script>
import MyComponent from './components/MyComponent.vue';
import Menu from './components/Menu.vue';

export default {
  components: {
    MyComponent,
    Menu
  }
};
</script>

<style>

</style>


