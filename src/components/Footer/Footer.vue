<template>
  <footer>{{ greeting }} World!</footer>
</template>

<script>
export default {
  setup() {
    return {
      greeting: 'Hello'
    };
  }
};
</script>

<style scoped>
footer {
  background: linear-gradient(130deg, #ff7a18, #af002d 41.07%, #319197 76.05%);
}
</style>