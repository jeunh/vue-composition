<template>
  <div>
    <p>{{ message }}</p>
    <button @click="changeMessage">change</button>
  </div>
</template>

<script>
import { ref } from 'vue';

  export default {
    setup() {
      // data
      const message = ref('hello');
      
      // methods
      function changeMessage() {
        message.value = 'hi';
      }

      return { message, changeMessage }
    }
  }
</script>

<style lang="scss" scoped>

</style>