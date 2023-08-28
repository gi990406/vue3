<template>
  <div class="name">
  {{ greet }}
  </div>
  <div class="justify-center flex bg-yellow-300 items-center h-screen">
    <div class="text-4xl">
      Hello, Tailwindcss
    </div>
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