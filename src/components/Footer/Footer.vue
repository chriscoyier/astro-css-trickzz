<script>
import { ref } from 'vue';
export default {
  setup() {
    const count = ref(0);
    const add = () => (count.value = count.value + 1);
    const subtract = () => (count.value = count.value - 1);
    return {
      count,
      add,
      subtract
    };
  }
};
</script>

<template>
  <footer>
    <button @click="subtract()">-</button>
    {{ count }}
    <button @click="add()">+</button>
  </footer>
</template>

<style scoped lang="scss">
footer {
  padding: 1rem;
  color: white;
  display: flex;
  justify-content: center;
  background: linear-gradient(130deg, #ff7a18, #af002d 41.07%, #319197 76.05%);
  > * {
    margin-inline: 1rem;
  }
}
</style>