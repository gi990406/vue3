<template>
  <div class="name">
  {{ greet }}
  </div>
</template>

<script>
export default {
    setup() {
      const name = 'knu1';

      const greeting = () => {
        return 'Hello, ' + name;
      };

      const greet = greeting(name);

      return {
        greet
      };
      
    }
}
</script>

<style>
  .name {
    color: red;
  }
</style>